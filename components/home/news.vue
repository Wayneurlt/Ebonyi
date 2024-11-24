<template>
  <section class="py-10 bg-gray-50 sm:py-16">
    <div class="px-4 mx-auto max-w-7xl sm:px-6 lg:px-8">
      <div class="text-center">
        <h2 class="text-3xl font-bold text-black sm:text-4xl lg:text-5xl">
          Latest News & Updates
        </h2>
        <p class="mt-4 text-base text-gray-600">
          Stay updated with the latest news, stories, and announcements about
          the Ebonyi diaspora in Kenya.
        </p>
      </div>

      <div class="grid gap-10 mt-10 md:grid-cols-2 lg:grid-cols-3">
        <!-- Featured Story -->
        <div class="overflow-hidden bg-white shadow-md transform transition-transform duration-300 hover:scale-105">
          <img
            class="object-cover w-full h-56"
            src="/assets/images/nigeriacap.jpg"
            alt="News 1"
          />
          <div class="p-6">
            <h3 class="text-xl font-semibold text-black">
              Ebonyi Cultural Festival in Nairobi
            </h3>
            <p class="mt-3 text-sm text-gray-600">
              Join us for the upcoming cultural festival showcasing traditional
              dances, foods, and more.
            </p>
            <a
              href="#"
              class="inline-block mt-4 text-sm font-medium text-green-600 hover:text-green-700 flex items-center gap-1 group"
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
        <div class="overflow-hidden bg-white shadow-md transform transition-transform duration-300 hover:scale-105">
          <img
            class="object-cover w-full h-56"
            src="/assets/images/peace.jpg"
            alt="News 2"
          />
          <div class="p-6">
            <h3 class="text-xl font-semibold text-black">
              Celebrating Achievements
            </h3>
            <p class="mt-3 text-sm text-gray-600">
              Meet Chinedu, who recently graduated with honors in Kenya. A proud
              moment for the community!
            </p>
            <a
              href="#"
              class="inline-block mt-4 text-sm font-medium text-green-600 hover:text-green-700 flex items-center gap-1 group"
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
        <div class="overflow-hidden bg-white shadow-md transform transition-transform duration-300 hover:scale-105">
          <img
            class="object-cover w-full h-56"
            src="/assets/images/nigeriacap.jpg"
            alt="News 3"
          />
          <div class="p-6">
            <h3 class="text-xl font-semibold text-black">
              Annual General Meeting Announced
            </h3>
            <p class="mt-3 text-sm text-gray-600">
              Mark your calendar for the Annual General Meeting to discuss plans
              and progress.
            </p>
            <a
              href="#"
              class="inline-block mt-4 text-sm font-medium text-green-600 hover:text-green-700 flex items-center gap-1 group"
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
</template>
