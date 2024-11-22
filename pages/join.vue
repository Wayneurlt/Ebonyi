<template>
  <section class="w-full h-screen bg-white">
    <div class="h-full w-full grid grid-cols-1 lg:grid-cols-2">
      <!-- Left Section -->
      <div
        class="relative flex items-end px-4 pb-10 pt-60 sm:pb-16 md:justify-center lg:pb-24 bg-gray-50 sm:px-6 lg:px-8"
      >
        <div class="absolute inset-0">
          <img
            class="object-cover object-top w-full h-full"
            src="/assets/images/peace.jpg"
            alt="Ebonyi Community"
          />
        </div>
        <div
          class="absolute inset-0 bg-gradient-to-t from-black to-transparent"
        ></div>

        <div class="relative">
          <div
            class="w-full max-w-xl xl:w-full xl:mx-auto xl:pr-24 xl:max-w-xl"
          >
            <h3 class="text-4xl font-bold text-white">
              Connect with the Ebonyi Community in Kenya
            </h3>
            <p class="mt-4 text-lg text-gray-200">
              Become part of a supportive network that celebrates our heritage,
              fosters growth, and creates opportunities.
            </p>
            <ul class="grid grid-cols-1 mt-10 sm:grid-cols-2 gap-x-8 gap-y-4">
              <li class="flex items-center space-x-3">
                <div
                  class="inline-flex items-center justify-center flex-shrink-0 w-5 h-5 bg-green-500 rounded-full"
                >
                  <svg
                    class="w-3.5 h-3.5 text-white"
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 20 20"
                    fill="currentColor"
                  >
                    <path
                      fill-rule="evenodd"
                      d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z"
                      clip-rule="evenodd"
                    ></path>
                  </svg>
                </div>
                <span class="text-lg font-medium text-white">
                  Exclusive Events
                </span>
              </li>
              <li class="flex items-center space-x-3">
                <div
                  class="inline-flex items-center justify-center flex-shrink-0 w-5 h-5 bg-green-500 rounded-full"
                >
                  <svg
                    class="w-3.5 h-3.5 text-white"
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 20 20"
                    fill="currentColor"
                  >
                    <path
                      fill-rule="evenodd"
                      d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z"
                      clip-rule="evenodd"
                    ></path>
                  </svg>
                </div>
                <span class="text-lg font-medium text-white">
                  Career Opportunities
                </span>
              </li>
              <li class="flex items-center space-x-3">
                <div
                  class="inline-flex items-center justify-center flex-shrink-0 w-5 h-5 bg-green-500 rounded-full"
                >
                  <svg
                    class="w-3.5 h-3.5 text-white"
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 20 20"
                    fill="currentColor"
                  >
                    <path
                      fill-rule="evenodd"
                      d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z"
                      clip-rule="evenodd"
                    ></path>
                  </svg>
                </div>
                <span class="text-lg font-medium text-white">
                  Cultural Workshops
                </span>
              </li>
              <li class="flex items-center space-x-3">
                <div
                  class="inline-flex items-center justify-center flex-shrink-0 w-5 h-5 bg-green-500 rounded-full"
                >
                  <svg
                    class="w-3.5 h-3.5 text-white"
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 20 20"
                    fill="currentColor"
                  >
                    <path
                      fill-rule="evenodd"
                      d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z"
                      clip-rule="evenodd"
                    ></path>
                  </svg>
                </div>
                <span class="text-lg font-medium text-white">
                  Social Support Network
                </span>
              </li>
            </ul>
          </div>
        </div>
      </div>

      <!-- Right Section -->
      <div
  class="flex items-center justify-center px-4 py-10 bg-white sm:px-6 lg:px-8 sm:py-16 lg:py-24"
>
  <div class="xl:w-full xl:max-w-sm 2xl:max-w-md xl:mx-auto">
    <h2 class="text-3xl font-bold leading-tight text-black sm:text-4xl">
      Join Us Today
    </h2>
    <p class="mt-2 text-base text-gray-600">
      Fill in your details to become part of our growing community.
    </p>

    <form action="#" method="POST" class="mt-8">
      <div class="space-y-5">
        <div>
          <label for="name" class="text-base font-medium text-gray-900">
            Full Name
          </label>
          <input
            type="text"
            id="name"
            placeholder="Enter your full name"
            class="block w-full mt-2.5 py-4 px-4 text-black placeholder-gray-500 border border-gray-200 rounded-md bg-gray-50 focus:outline-none focus:border-green-600 focus:bg-white caret-green-600"
          />
        </div>

        <div>
          <label for="email" class="text-base font-medium text-gray-900">
            Email Address
          </label>
          <input
            type="email"
            id="email"
            placeholder="Enter your email"
            class="block w-full mt-2.5 py-4 px-4 text-black placeholder-gray-500 border border-gray-200 rounded-md bg-gray-50 focus:outline-none focus:border-green-600 focus:bg-white caret-green-600"
          />
        </div>

        <div>
          <label for="phone" class="text-base font-medium text-gray-900">
            Phone Number
          </label>
          <input
            type="tel"
            id="phone"
            placeholder="Enter your phone number (e.g., +123456789)"
            class="block w-full mt-2.5 py-4 px-4 text-black placeholder-gray-500 border border-gray-200 rounded-md bg-gray-50 focus:outline-none focus:border-green-600 focus:bg-white caret-green-600"
          />
        </div>

        <div>
          <button
            type="submit"
            class="inline-flex items-center justify-center w-full px-4 py-4 text-base font-semibold text-white transition-all duration-200 bg-green-600 rounded-md focus:outline-none hover:bg-green-700"
          >
            Join the Community
          </button>
        </div>
      </div>
    </form>
  </div>
</div>

    </div>
  </section>
</template>
