<template>
  <footer
    class="font-lexend py-4 w-full min-h-full bg-green-100 dark:bg-green-500"
  >
    <div class="max-w-[80rem] mx-auto space-y-6 px-2 md:px-4 lg:px-6 pt-4">
      <div
        class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-5 gap-6 md:gap-y-6"
      >
        <div class="text-black dark:text-white">
          <ul>
            <li class="mb-4">
              <h2 class="font-bold text-lg">Resources</h2>
            </li>
            <li><a href="/services">Our Services</a></li>
            <li><a href="/programs">Community Programs</a></li>
            <li><a href="/events">Upcoming Events</a></li>
            <li><a href="/support">Support</a></li>
          </ul>
        </div>
        <div class="text-black dark:text-white">
          <ul>
            <li class="mb-4">
              <h2 class="font-bold text-lg">Quick Links</h2>
            </li>
            <li><a href="/about">About Us</a></li>
            <li><a href="/blog">Blog</a></li>
            <li><a href="/contact">Contact</a></li>
          </ul>
        </div>
        <div class="text-black dark:text-white">
          <ul>
            <li class="mb-4">
              <h2 class="font-bold text-lg">The Organization</h2>
            </li>
            <li><a href="/mission">Our Mission</a></li>
            <li><a href="/team">Our Team</a></li>
            <li><a href="/careers">Careers</a></li>
          </ul>
        </div>
        <div class="bg-green-200 dark:bg-green-600 lg:col-span-2 p-4 space-y-2">
          <h2 class="font-bold text-lg text-black dark:text-white">
            Stay Connected
          </h2>
          <div
            class="relative flex flex-row w-full rounded-xl overflow-hidden border h-12"
          >
            <label for="email" class="sr-only">Email</label>
            <input
              type="email"
              id="email"
              placeholder="yourname@example.com"
              class="flex-1 bg-white text-black h-full px-4 focus:border-none focus:outline-none focus:ring-0"
            />
            <button
  type="submit"
  class="inline-block h-full px-3 w-12 md:w-16 bg-green-600 text-white group"
>
  <svg
    xmlns="http://www.w3.org/2000/svg"
    class="w-6 h-full fill-current mx-auto transition-transform duration-200 group-hover:translate-x-2"
    viewBox="0 0 512 512"
  >
    <path
      d="M502.6 278.6c12.5-12.5 12.5-32.8 0-45.3l-128-128c-12.5-12.5-32.8-12.5-45.3 0s-12.5 32.8 0 45.3L402.7 224 32 224c-17.7 0-32 14.3-32 32s14.3 32 32 32l370.7 0-73.4 73.4c-12.5 12.5-12.5 32.8 0 45.3s32.8 12.5 45.3 0l128-128z"
    />
  </svg>
</button>

          </div>
          <p class="max-w-96 text-white font-light">
            Join our newsletter to stay updated on our latest initiatives and
            events aimed at supporting the Ebonyi community in Kenya.
          </p>
        </div>
      </div>
      <div class="h-px w-full bg-gray-300"></div>
      <div
        class="flex flex-row justify-between items-center text-sm text-white"
      >
        <a href="/" class="inline-flex items-center gap-1">
          <img src="/public/logo.png" alt="Ebonyi Kenya Logo" class="h-20" />
        </a>

        <ul class="flex items-center gap-4">
          <li><a href="/privacy" class="inline-block">Privacy Policy</a></li>
          <li>
            <a href="/terms" class="inline-block">Terms and Conditions</a>
          </li>
        </ul>

        <ul class="flex items-center gap-4">
          <li>
            <a
              href="https://facebook.com"
              class="inline-block rounded-full h-8 w-8 p-2 border"
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                class="w-full h-full fill-current"
                viewBox="0 0 512 512"
              >
                <path
                  d="M504 256C504 119 393 8 256 8S8 119 8 256c0 123.8 89.7 226.2 208 248v-176h-62v-72h62v-56c0-61.9 37-96 93.7-96 27.3 0 56 5 56 5v61h-31.6c-31.1 0-40.4 19.4-40.4 39.3v47.7h69l-11 72h-58v176c118.3-21.8 208-124.2 208-248z"
                />
              </svg>
            </a>
          </li>
          <li>
            <a
              href="https://twitter.com"
              class="inline-block rounded-full h-8 w-8 p-2 border"
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                class="w-full h-full fill-current"
                viewBox="0 0 512 512"
              >
                <path
                  d="M459.4 151.7c.3 4.5.3 9.1.3 13.7 0 140.7-107.1 303.5-303.5 303.5-60.4 0-116.7-17.6-164.3-48 8.5 1 16.9 1.3 25.6 1.3a215.5 215.5 0 0 0 133.6-46.1c-41.6-.8-77.1-28.2-89.3-65.8 5.8.8 11.6 1.6 17.8 1.6 8.4 0 16.6-1.1 24.4-3-43.3-8.7-76-47.3-76-93.7v-1.2c12.9 7.2 28.1 11.6 44.3 12.1a93.4 93.4 0 0 1-28.8-124.6 265 265 0 0 0 192.4 97.6c-6.8-33.1 5-67.4 31.3-87.5 26.3-20.1 63.5-20.6 92.1-1.6 14.7-2.9 28.6-8.3 41.1-15.7-4.9 15.4-15.4 28.3-29.1 36.4 13-.7 25.5-5 37-10.1-8.7 12.7-19.6 23.6-31.8 32.4z"
                />
              </svg>
            </a>
          </li>
        </ul>
      </div>
    </div>
  </footer>
</template>
