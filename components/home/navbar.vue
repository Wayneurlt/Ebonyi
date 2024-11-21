<template>
  <nav
    :class="[ 
      'px-8 py-3 xl:py-4 fixed top-0 w-full z-[1000]',
      {
        'dark:bg-white bg-satinlinen': isScrolled,
        'bg-transparent': !isScrolled,
      },
    ]"
  >
    <div class="flex justify-between w-full place-items-center">
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




      <!-- Actions and Links on the Right -->
      <div class="flex items-center gap-5">
        <NuxtLink to="/product-catalog" class="font-semibold">
          About Us
        </NuxtLink>
        <div class="w-full h-full mt-2">
          <ThemeSwitch />
        </div>
        <NuxtLink
          to="/auth/login"
          class="grid place-items-center px-4 py-2 bg-transparent border border-black dark:border-black text-black dark:text-black rounded-full focus:outline-none focus:ring-4 focus:ring-green-500 whitespace-nowrap transition-all"
          >Join Us</NuxtLink
        >
      </div>
    </div>
  </nav>
</template>

<script setup lang="ts">
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
</script>

<style>
.item-hover:hover .move-left {
  transform: translateX(5px);
  opacity: 1;
  transition: transform 0.4s ease-in-out, opacity 0.4s ease-in-out;
  cursor: pointer;
}
</style>
