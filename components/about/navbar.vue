<template>
  <nav >
    <div class="flex justify-between items-center w-full bg-white px-6 py-4">
  <!-- Enlarged Logo on the Left -->
  <NuxtLink to="/" class="flex items-center">
    <ClientOnly>
      <img
        class="h-12 lg:h-24 xl:h-18 2xl:h-21 w-auto"
        src="/public/logo.png"
        alt="Logo"
      />
    </ClientOnly>
  </NuxtLink>

  <div class="flex items-center gap-5">
   

    <NuxtLink
      to="/about"
      class="font-semibold transition-transform transform hover:scale-105"
    >
      About Us
    </NuxtLink>

    <NuxtLink
      to="/join"
      class="grid place-items-center px-6 py-3 bg-green-500 text-white rounded-full focus:outline-none focus:ring-4 focus:ring-green-500 whitespace-nowrap transition-all transform hover:scale-105"
    >
      Join Us
    </NuxtLink>
  </div>
</div>

  </nav>
</template>

<!-- <script setup lang="ts">
let isScrolled = ref(false);

onMounted(() => {
  window.addEventListener("scroll", () => {
    isScrolled.value = window.scrollY > 0;
  });
});

const colorMode = useColorMode();
const isDark = computed({
  get() {
    return colorMode.value === "dark";
  },
  set() {
    colorMode.preference = colorMode.value === "dark" ? "light" : "dark";
  },
});
</script> -->
<!-- 
<style>
.item-hover:hover .move-left {
  transform: translateX(5px);
  opacity: 1;
  transition: transform 0.4s ease-in-out, opacity 0.4s ease-in-out;
  cursor: pointer;
}
</style> -->
