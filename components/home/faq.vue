<template>
  <section class="py-10 sm:py-16 lg:py-12 bg-white">
    <div class="px-4 mx-auto sm:px-6 lg:px-8 max-w-7xl">
      <div class="max-w-2xl mx-auto text-center">
        <h2 class="text-3xl font-bold leading-tight sm:text-4xl lg:text-5xl">
          Frequently Asked Questions
        </h2>
      </div>
      <div
        class="max-w-3xl mx-auto mt-4 space-y-4 md:mt-16 border border-gray-200 z-[100] relative"
      >
        <div
          class="transition-all duration-200 shadow-lg cursor-pointer 2xl:ext-xl"
        >
          <button
            @click="activeIndex == 1 ? (activeIndex = 0) : (activeIndex = 1)"
            class="flex justify-between w-full px-4 py-5 sm:p-6 gap-3"
          >
            <span class="flex 2xl:text-2xl text-start font-semibold">
              How can I join the Ebonyi Diaspora community in Kenya?
            </span>

            <svg
              :class="{ 'rotate-180': activeIndex === 1 }"
              class="w-6 h-6 text-gray-400"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M19 9l-7 7-7-7"
              />
            </svg>
          </button>
          <div v-if="activeIndex === 1" class="px-4 pb-5 sm:px-6 sm:pb-6">
            <p>
              Joining the Ebonyi Diaspora in Kenya is easy! Simply
              <NuxtLink to="/join" title="" class="underline"
                >sign up on our platform</NuxtLink
              >
              , provide your details, and become part of a vibrant network of
              Ebonyi indigenes dedicated to preserving our culture and building
              a supportive community.
            </p>
          </div>
        </div>
        <div
          class="transition-all duration-200 shadow-lg cursor-pointer 2xl:text-xl"
        >
          <button
            @click="activeIndex == 2 ? (activeIndex = 0) : (activeIndex = 2)"
            class="flex justify-between w-full px-4 py-5 sm:p-6 cursor-pointer gap-3"
          >
            <span
              class="flex 2xl:text-2xl font-semibold text-start cursor-pointer"
            >
              What events do you organize for Ebonyi indigenes?
            </span>

            <svg
              :class="{ 'rotate-180': activeIndex === 2 }"
              class="w-6 h-6 text-gray-400"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M19 9l-7 7-7-7"
              />
            </svg>
          </button>

          <div v-if="activeIndex === 2" class="px-4 pb-5 sm:px-6 sm:pb-6">
            <p>
              We host a variety of events, including cultural festivals,
              networking forums, business expos, and charity drives aimed at
              empowering Ebonyi indigenes and celebrating our heritage.
            </p>
          </div>
        </div>
        <div
          class="transition-all duration-200 shadow-lg cursor-pointer 2xl:text-xl"
        >
          <button
            @click="activeIndex == 3 ? (activeIndex = 0) : (activeIndex = 3)"
            class="flex justify-between w-full px-4 py-5 sm:p-6 cursor-pointer gap-3"
          >
            <span
              class="flex 2xl:text-2xl font-semibold text-start cursor-pointer"
            >
              How does the community support members?
            </span>

            <svg
              :class="{ 'rotate-180': activeIndex === 3 }"
              class="w-6 h-6 text-gray-400"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M19 9l-7 7-7-7"
              />
            </svg>
          </button>

          <div v-if="activeIndex === 3" class="px-4 pb-5 sm:px-6 sm:pb-6">
            <p>
              We provide support through mentorship programs, business
              networking opportunities, cultural exchange, and access to
              resources that help members grow personally and professionally.
            </p>
          </div>
        </div>
        <div
          class="transition-all duration-200 shadow-lg cursor-pointer 2xl:text-xl"
        >
          <button
            @click="activeIndex == 4 ? (activeIndex = 0) : (activeIndex = 4)"
            class="flex justify-between w-full px-4 py-5 sm:p-6 cursor-pointer gap-3"
          >
            <span
              class="flex 2xl:text-2xl font-semibold text-start cursor-pointer"
            >
              What are the membership benefits?
            </span>

            <svg
              :class="{ 'rotate-180': activeIndex === 4 }"
              class="w-6 h-6 text-gray-400"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M19 9l-7 7-7-7"
              />
            </svg>
          </button>

          <div v-if="activeIndex === 4" class="px-4 pb-5 sm:px-6 sm:pb-6">
            <p>
              Membership benefits include access to exclusive events, cultural
              preservation initiatives, community projects, professional growth
              opportunities, and a strong support network of fellow Ebonyi
              indigenes.
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
let activeIndex = ref(0);
</script>
