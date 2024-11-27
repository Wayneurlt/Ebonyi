<template>
  <AboutNavbar />
  <div
    ref="canvasContainerRef"
    class="fixed inset-0 w-full h-full overflow-hidden"
    aria-hidden="true"
  >
    <canvas ref="canvasRef" class="w-full h-full"></canvas>
  </div>
 








  <section class="py-10 bg-transparent sm:py-16">
    <div class="px-4 mx-auto max-w-7xl sm:px-6 lg:px-8">

      <div class="grid gap-10 mt-10 md:grid-cols-2 lg:grid-cols-3">
        <!-- Featured Story -->
        <div class="overflow-hidden bg-transparent shadow-md transform transition-transform duration-300 hover:scale-105">
          <img
            class="object-cover w-full h-56"
            src="/assets/images/ebony.webp"
            alt="News 1"
          />
          <div class="p-6">
            <h3 class="text-xl font-semibold text-green-500">
              Ebonyi Cultural Festival in Nairobi
            </h3>
            <p class="mt-3 text-sm text-white">
              Join us for the upcoming cultural festival showcasing traditional
              dances, foods, and more.
            </p>
            <a
              href="#"
              class=" mt-4 text-sm font-medium text-green-600 hover:text-green-700 flex items-center gap-1 group"
            >
              Read more
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke-width="2"
                stroke="currentColor"
                class="w-4 h-4 transform transition-transform duration-300 group-hover:translate-x-1"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M9 5l7 7-7 7"
                />
              </svg>
            </a>
          </div>
        </div>

        <!-- News Article -->
        <div class="overflow-hidden bg-transparent shadow-md transform transition-transform duration-300 hover:scale-105">
          <img
            class="object-cover w-full h-56"
            src="/assets/images/peace.jpg"
            alt="News 2"
          />
          <div class="p-6">
            <h3 class="text-xl font-semibold text-green-500">
              Celebrating Achievements
            </h3>
            <p class="mt-3 text-sm text-white">
              Meet Chinedu, who recently graduated with honors in Kenya. A proud
              moment for the community!
            </p>
            <a
              href="#"
              class=" mt-4 text-sm font-medium text-green-600 hover:text-green-700 flex items-center gap-1 group"
            >
              Read more
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke-width="2"
                stroke="currentColor"
                class="w-4 h-4 transform transition-transform duration-300 group-hover:translate-x-1"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M9 5l7 7-7 7"
                />
              </svg>
            </a>
          </div>
        </div>

        <!-- Announcement -->
        <div class="overflow-hidden bg-transparent shadow-md transform transition-transform duration-300 hover:scale-105">
          <img
            class="object-cover w-full h-56"
            src="/assets/images/ebonya.webp"
            alt="News 3"
          />
          <div class="p-6">
            <h3 class="text-xl font-semibold text-green-500">
              Annual General Meeting Announced
            </h3>
            <p class="mt-3 text-sm text-white">
              Mark your calendar for the Annual General Meeting to discuss plans
              and progress.
            </p>
            <a
              href="#"
              class=" mt-4 text-sm font-medium text-green-600 hover:text-green-700 flex items-center gap-1 group"
            >
              Read more
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke-width="2"
                stroke="currentColor"
                class="w-4 h-4 transform transition-transform duration-300 group-hover:translate-x-1"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M9 5l7 7-7 7"
                />
              </svg>
            </a>
          </div>
        </div>
      </div>
    </div>
  </section>



 























<HomeFoot/>
</template>

<script setup lang="ts">
import { HomeNavbar } from "#build/components";
import { useMouse, useDevicePixelRatio } from "@vueuse/core";

type Circle = {
  x: number;
  y: number;
  translateX: number;
  translateY: number;
  size: number;
  alpha: number;
  targetAlpha: number;
  dx: number;
  dy: number;
  magnetism: number;
};

type Props = {
  color?: string;
  quantity?: number;
  staticity?: number;
  ease?: number;
  class?: string;
};

const props = withDefaults(defineProps<Props>(), {
  color: "#FFF",
  quantity: 200,
  staticity: 50,
  ease: 50,
  class: "",
});

const canvasRef = ref<HTMLCanvasElement | null>(null);
const canvasContainerRef = ref<HTMLDivElement | null>(null);
const context = ref<CanvasRenderingContext2D | null>(null);
const circles = ref<Circle[]>([]);
const mouse = reactive<{ x: number; y: number }>({ x: 0, y: 0 });
const canvasSize = reactive<{ w: number; h: number }>({ w: 0, h: 0 });
const { x: mouseX, y: mouseY } = useMouse();
const { pixelRatio } = useDevicePixelRatio();

const color = computed(() => {
  // Remove the leading '#' if it's present
  let hex = props.color.replace(/^#/, "");

  // If the hex code is 3 characters, expand it to 6 characters
  if (hex.length === 3) {
    hex = hex
      .split("")
      .map((char) => char + char)
      .join("");
  }

  // Parse the r, g, b values from the hex string
  const bigint = parseInt(hex, 16);
  const r = (bigint >> 16) & 255; // Extract the red component
  const g = (bigint >> 8) & 255; // Extract the green component
  const b = bigint & 255; // Extract the blue component

  // Return the RGB values as a string separated by spaces
  return `${r} ${g} ${b}`;
});

onMounted(() => {
  if (canvasRef.value) {
    context.value = canvasRef.value.getContext("2d");
  }

  initCanvas();
  animate();
  window.addEventListener("resize", initCanvas);
});

onBeforeUnmount(() => {
  window.removeEventListener("resize", initCanvas);
});

watch([mouseX, mouseY], () => {
  onMouseMove();
});

function initCanvas() {
  resizeCanvas();
  drawParticles();
}

function onMouseMove() {
  if (canvasRef.value) {
    const rect = canvasRef.value.getBoundingClientRect();
    const { w, h } = canvasSize;
    const x = mouseX.value - rect.left - w / 2;
    const y = mouseY.value - rect.top - h / 2;

    const inside = x < w / 2 && x > -w / 2 && y < h / 2 && y > -h / 2;
    if (inside) {
      mouse.x = x;
      mouse.y = y;
    }
  }
}

function resizeCanvas() {
  if (canvasContainerRef.value && canvasRef.value && context.value) {
    circles.value.length = 0;
    canvasSize.w = canvasContainerRef.value.offsetWidth;
    canvasSize.h = canvasContainerRef.value.offsetHeight;
    canvasRef.value.width = canvasSize.w * pixelRatio.value;
    canvasRef.value.height = canvasSize.h * pixelRatio.value;
    canvasRef.value.style.width = canvasSize.w + "px";
    canvasRef.value.style.height = canvasSize.h + "px";
    context.value.scale(pixelRatio.value, pixelRatio.value);
  }
}

function circleParams(): Circle {
  const x = Math.floor(Math.random() * canvasSize.w);
  const y = Math.floor(Math.random() * canvasSize.h);
  const translateX = 0;
  const translateY = 0;
  const size = Math.floor(Math.random() * 2) + 1;
  const alpha = 0;
  const targetAlpha = parseFloat((Math.random() * 0.6 + 0.1).toFixed(1));
  const dx = (Math.random() - 0.5) * 10;
  const dy = (Math.random() - 0.5) * 10;
  const magnetism = 0.1 + Math.random() * 4;
  return {
    x,
    y,
    translateX,
    translateY,
    size,
    alpha,
    targetAlpha,
    dx,
    dy,
    magnetism,
  };
}

function drawCircle(circle: Circle, update = false) {
  if (context.value) {
    const { x, y, translateX, translateY, size, alpha } = circle;
    context.value.translate(translateX, translateY);
    context.value.beginPath();
    context.value.arc(x, y, size, 0, 2 * Math.PI);
    context.value.fillStyle = `rgba(${color.value
      .split(" ")
      .join(", ")}, ${alpha})`;
    context.value.fill();
    context.value.setTransform(pixelRatio.value, 0, 0, pixelRatio.value, 0, 0);

    if (!update) {
      circles.value.push(circle);
    }
  }
}

function clearContext() {
  if (context.value) {
    context.value.clearRect(0, 0, canvasSize.w, canvasSize.h);
  }
}

function drawParticles() {
  clearContext();
  const particleCount = props.quantity;
  for (let i = 0; i < particleCount; i++) {
    const circle = circleParams();
    drawCircle(circle);
  }
}

function remapValue(
  value: number,
  start1: number,
  end1: number,
  start2: number,
  end2: number
): number {
  const remapped =
    ((value - start1) * (end2 - start2)) / (end1 - start1) + start2;
  return remapped > 0 ? remapped : 0;
}

function animate() {
  clearContext();
  circles.value.forEach((circle, i) => {
    // Handle the alpha value
    const edge = [
      circle.x + circle.translateX - circle.size, // distance from left edge
      canvasSize.w - circle.x - circle.translateX - circle.size, // distance from right edge
      circle.y + circle.translateY - circle.size, // distance from top edge
      canvasSize.h - circle.y - circle.translateY - circle.size, // distance from bottom edge
    ];

    const closestEdge = edge.reduce((a, b) => Math.min(a, b));
    const remapClosestEdge = parseFloat(
      remapValue(closestEdge, 0, 20, 0, 1).toFixed(2)
    );

    if (remapClosestEdge > 1) {
      circle.alpha += 0.02;
      if (circle.alpha > circle.targetAlpha) circle.alpha = circle.targetAlpha;
    } else {
      circle.alpha = circle.targetAlpha * remapClosestEdge;
    }

    circle.x += circle.dx;
    circle.y += circle.dy;
    circle.translateX +=
      (mouse.x / (props.staticity / circle.magnetism) - circle.translateX) /
      props.ease;
    circle.translateY +=
      (mouse.y / (props.staticity / circle.magnetism) - circle.translateY) /
      props.ease;

    // circle gets out of the canvas
    if (
      circle.x < -circle.size ||
      circle.x > canvasSize.w + circle.size ||
      circle.y < -circle.size ||
      circle.y > canvasSize.h + circle.size
    ) {
      // remove the circle from the array
      circles.value.splice(i, 1);
      // create a new circle
      const newCircle = circleParams();
      drawCircle(newCircle);
      // update the circle position
    } else {
      drawCircle(
        {
          ...circle,
          x: circle.x,
          y: circle.y,
          translateX: circle.translateX,
          translateY: circle.translateY,
          alpha: circle.alpha,
        },
        true
      );
    }
  });
  window.requestAnimationFrame(animate);
}
</script>
