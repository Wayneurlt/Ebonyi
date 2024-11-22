<template>
    <div class="flex items-center justify-center">
      <FlipCard
        description="Inspira UI offers beautifully designed, reusable animation components and includes custom components developed by us and contributed by the community."
        image=" https://images.unsplash.com/photo-1525373698358-041e3a460346?w=600&auto=format&fit=crop&q=60&ixlib=rb-4.0.3"
        rotate="y"
        subtitle="What is Inspira UI?"
        title="Inspira UI"
      />
    </div>
  </template>
<!-- <script setup lang="ts">
import alphaImage from '../../assets/images/alpha.jpeg';
import officeClean   from '../../assets/images/officeclean.jpg';
import outreach from '../../assets/images/outreach.jpg'
import plumber  from '../../assets/images/plumber.jpg';
import cook  from '../../assets/images/cook.jpg';
import cleanOffice  from '../../assets/images/cleanoffice.jpg';
import portrait  from '../../assets/images/portrait.jpg';
import accelerator  from '../../assets/images/accelerator.jpg';
import work  from '../../assets/images/work.jpg';
import outreachClean from '../../assets/images/outreachclean3.jpg';

const items = [
  {
    src: alphaImage,
  },
  {
    src: officeClean,
  },
  {
    src: outreach,
  },
  {
    src: plumber,
  },
  {
    src: cook,
  },
  {
    src: cleanOffice
  },
  {
    src: portrait
  },
  {
    src: accelerator
  },
  {
    src: work
  },
  {
    src: outreachClean
  },
];
</script>

<template>
  <div class="carousel-container bg-black">
    <div class="carousel-track">
      <div
        v-for="(item, index) in items"
        :key="`original-${index}`"
        class="carousel-item"
      >
        <div class="relative">
          <div
            class="absolute h-full w-full flex text-white gap-4 cooperated"
          ></div>
          <img
            :src="item.src"
            class="2xl:h-96 lg:h-72 h-64 w-auto object-cover rounded-xl"
            draggable="false"
          />
        </div>
      </div>
      <div
        v-for="(item, index) in items"
        :key="`duplicate-${index}`"
        class="carousel-item"
      >
        <div class="relative">
          <div
            v-if="index == 3 || index == 5"
            class="absolute h-full w-full flex text-white gap-4 cooperated"
          >
            <div
              class="flex gap-2 lg:py-5 lg:px-6 py-2 px-2 h-full flex-col"
            ></div>
          </div>
          <img
            :src="item.src"
            class="2xl:h-96 lg:h-72 h-64 w-auto object-cover rounded-xl"
            draggable="false"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.carousel-container {
  overflow: hidden;
  width: 100%;
}
.carousel-container:hover .carousel-track {
  animation-play-state: paused;
}

.carousel-item {
  flex: 0 0 auto;
}

.carousel-item img {
  display: block;
}

.carousel-track {
  display: flex;
  gap: 1rem;
  width: calc(2 * 100% + 20px);
  animation: scroll 45s linear infinite;
}

@media (max-width: 768px) {
  .carousel-track {
    display: flex;
    gap: 0.5rem;
    width: calc(450% + 20px);
    animation: scrollM 120s linear infinite;
  }
}

@keyframes scroll {
  0% {
    transform: translate3d(0, 0, 0); /* Using transform for hardware acceleration */
  }
  100% {
    transform: translate3d(calc(-100% - 20px), 0, 0); /* Using transform for hardware acceleration */
  }
}

@keyframes scrollM {
  0% {
    transform: translate3d(0, 0, 0); /* Using transform for hardware acceleration */
  }
  100% {
    transform: translate3d(calc(-400% - 20px), 0, 0); /* Using transform for hardware acceleration */
  }
}

</style> -->
