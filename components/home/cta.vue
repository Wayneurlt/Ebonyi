<template>

<section class="py-10 bg-white sm:py-16 lg:py-24">
  <div class="px-4 mx-auto max-w-7xl sm:px-6 lg:px-8">
    <div class="grid items-stretch gap-y-10 md:grid-cols-2 md:gap-x-20">
      <!-- Images Section -->
      <div class="relative grid grid-cols-2 gap-6 mt-10 md:mt-0">
        <div class="overflow-hidden aspect-w-3 aspect-h-4  ">
          <img
            class="object-cover object-top origin-top scale-150 "
            src="/assets/images/nigeriacap.jpg"
            alt="Nigerian Cap"
          />
        </div>

        <div class="relative">
          <div class="h-full overflow-hidden aspect-w-3 aspect-h-4 ">
            <img
              class="object-cover scale-150 lg:origin-bottom-right "
              src="/assets/images/nige.jpg"
              alt="Nigerian Cap Close-Up"
            />
          </div>
        </div>
      </div>

      <!-- CTA Section -->
      <div class="flex flex-col items-start xl:px-16">
        <h2 class="text-3xl font-bold leading-tight text-black sm:text-4xl lg:text-5xl">
          Unite with Ebonyi in Kenya
        </h2>
        <p class="mt-4 text-base leading-relaxed text-gray-600">
          Join the Ebonyi diaspora in Kenya to celebrate our shared heritage,
          connect with fellow members, and participate in exciting cultural
          events. Together, we preserve the beauty of Ebonyi's traditions while
          building a vibrant, supportive community.
        </p>

        <a
          href="/join"
          title="Join the Ebonyi Community"
          class="inline-flex items-center justify-center px-5 py-4 mt-8 text-base font-semibold text-white transition-all duration-200 rounded-md hover:opacity-90 focus:opacity-90 lg:mt-auto bg-gradient-to-r from-green-600 to-black"
          role="button"
        >
          Join Us Now
          <svg
            class="w-5 h-5 ml-8 -mr-1"
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M10.293 3.293a1 1 0 011.414 0l6 6a1 1 0 010 1.414l-6 6a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-4.293-4.293a1 1 0 010-1.414z"
              clip-rule="evenodd"
            />
          </svg>
        </a>
      </div>
    </div>
  </div>
</section>







</template>