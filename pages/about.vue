<template>
  <!DOCTYPE html>
  <html lang="en">
    <body class="bg-gray-50 text-gray-800">
      <!-- Hero Section -->
      <div class="relative h-[32rem]">
        <!-- Image Background -->
        <img
          src="/assets/images/bg.webp"
          alt="Background Image"
          class="absolute inset-0 w-full h-full object-cover"
        />

        <!-- Overlay -->
        <div
          class="absolute inset-0 bg-gradient-to-t from-black/60 via-black/40 to-transparent"
        ></div>

        <!-- Text Content -->
        <div
          class="relative z-10 flex flex-col items-center justify-center h-full text-center text-white px-6 sm:px-12"
        >
          <h1
            class="text-4xl font-bold md:text-6xl opacity-0 translate-y-10 animate-fade-in-up"
          >
            About Us
          </h1>
          <p
            class="mt-4 text-lg opacity-90 translate-y-10 animate-fade-in-up"
          >
            Celebrating the people of Ebonyi in the diaspora here in Kenya.
          </p>
          <p
            class="mt-6 text-base sm:text-lg md:max-w-2xl lg:max-w-3xl opacity-0 translate-y-10 animate-fade-in-up"
          >
            We are a vibrant community of Ebonyi indigenes living in Kenya,
            united by a shared heritage and a commitment to supporting one
            another. Our mission is to foster growth, celebrate our culture, and
            create opportunities for every member of our diaspora family.
          </p>
        </div>
      </div>

      <!-- Mission and Vision Section -->
      <section class="py-16 px-6 bg-transparent sm:px-12 lg:px-20">
        <div class="py-20 bg-white">
          <div class="xl:container mx-auto px-6 md:px-12">
            <div class="mb-16 md:w-2/3 lg:w-1/2 text-center mx-auto">
              <h2 class="mb-4 text-2xl font-bold text-black md:text-4xl">
                Our Mission and Vision
              </h2>
              <p>yeahhhhhh</p>
            </div>

            <div class="grid gap-6 px-4 sm:px-0 sm:grid-cols-1 md:grid-cols-2">
              <!-- Vision Tile -->
              <div
                class="group relative rounded-3xl space-y-6 overflow-hidden border border-green-500"
              >
                <img
                  class="mx-auto h-[26rem] w-full object-cover object-top transition duration-500 group-hover:scale-105"
                  src="/assets/images/vision.webp"
                  alt="Our Vision"
                  loading="lazy"
                  width="640"
                  height="805"
                />
                <div
                  class="absolute bottom-0 inset-x-0 h-max mt-auto px-8 py-6 bg-green-700 text-white translate-y-24 transition duration-300 ease-in-out group-hover:translate-y-0"
                >
                  <div>
                    <h4 class="text-xl font-semibold">Our Vision</h4>
                    <span class="block text-sm text-gray-200">
                      Celebrating Ebonyi heritage, inspiring unity
                    </span>
                  </div>
                  <p class="mt-8 text-gray-100">
                    "To unite and empower the Ebonyi Diaspora in Kenya by
                    fostering a community where culture, collaboration, and
                    progress thrive for a better tomorrow"
                  </p>
                </div>
              </div>

              <!-- Mission Tile -->
              <div
                class="group relative rounded-3xl space-y-6 overflow-hidden border border-green-500"
              >
                <img
                  class="mx-auto h-[26rem] w-full object-cover object-top transition duration-500 group-hover:scale-105"
                  src="/assets/images/nigeriacap.jpg"
                  alt="Our Mission"
                  loading="lazy"
                  width="640"
                  height="805"
                />
                <div
                  class="absolute bottom-0 inset-x-0 h-max mt-auto px-8 py-6 bg-green-700 text-white translate-y-24 transition duration-300 ease-in-out group-hover:translate-y-0"
                >
                  <div>
                    <h4 class="text-xl font-semibold">Our Mission</h4>
                    <span class="block text-sm text-gray-200">
                      Strengthening connections, uplifting communities
                    </span>
                  </div>
                  <p class="mt-8 text-gray-100">
                    "To create opportunities for Ebonyi indigenes in Kenya by
                    connecting resources, preserving traditions, and building a
                    foundation for future generations."
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>

      <!-- Team Section -->
      <section class="py-16 px-6 sm:px-12 lg:px-20">
        <div class="container mx-auto text-center">
          <h2
            class="text-3xl font-bold opacity-0 translate-y-10 animate-fade-in-up"
          >
            Meet the Leaders
          </h2>
          <p
            class="mt-4 text-lg text-gray-600 opacity-0 translate-y-10 animate-fade-in-up"
          >
            Our leadership team works tirelessly to bring the Ebonyi diaspora
            together, ensuring that every voice is heard and every member is
            supported.
          </p>
          <div
            class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8 mt-10"
          >
            <!-- Team Member -->
            <div class="opacity-0 translate-y-10 animate-fade-in-up">
              <img
                src="https://via.placeholder.com/400x400"
                alt="Leader"
                class="w-48 mx-auto"
              />
              <h3 class="mt-4 text-xl font-semibold">Nkechi Okoro</h3>
              <p class="text-gray-600">President</p>
            </div>
            <!-- Repeat Team Members -->
            <div class="opacity-0 translate-y-10 animate-fade-in-up">
              <img
                src="https://via.placeholder.com/400x400"
                alt="Leader"
                class="w-48 mx-auto"
              />
              <h3 class="mt-4 text-xl font-semibold">Emeka Nwankwo</h3>
              <p class="text-gray-600">Vice President</p>
            </div>
            <div class="opacity-0 translate-y-10 animate-fade-in-up">
              <img
                src="https://via.placeholder.com/400x400"
                alt="Leader"
                class="w-48 mx-auto"
              />
              <h3 class="mt-4 text-xl font-semibold">Chidera Mba</h3>
              <p class="text-gray-600">Cultural Coordinator</p>
            </div>
          </div>
        </div>
      </section>

      <section class="py-10 bg-white sm:py-16 lg:py-24">
        <div class="max-w-6xl px-4 mx-auto sm:px-6 lg:px-8">
          <div
            class="grid grid-cols-1 md:items-stretch md:grid-cols-2 gap-x-12 lg:gap-x-20 gap-y-10"
          >
            <!-- Contact Information -->
            <div class="flex flex-col justify-between lg:py-5">
              <div>
                <h2
                  class="text-3xl font-bold leading-tight text-green-600 sm:text-4xl lg:leading-tight lg:text-5xl"
                >
                  Stay Connected with Us
                </h2>
                <p
                  class="max-w-xl mx-auto mt-4 text-base leading-relaxed text-gray-700"
                >
                  Have questions or want to get involved? We're here to help.
                  Reach out to us, and let's celebrate the Ebonyi spirit
                  together.
                </p>
              </div>

              <div class="hidden md:mt-auto md:block">
                <blockquote class="mt-6">
                  <p class="text-lg leading-relaxed text-gray-600">
                    "Being part of this community has strengthened my connection
                    to home and created lifelong bonds."
                  </p>
                </blockquote>
                <div class="flex items-center mt-8">
                  <img
                    class="flex-shrink-0 object-cover w-10 h-10 rounded-full"
                    src="https://via.placeholder.com/150"
                    alt="Testimonial"
                  />
                  <div class="ml-4">
                    <p class="text-base font-semibold text-green-600">
                      Chidera Okonkwo
                    </p>
                    <p class="mt-px text-sm text-gray-500">
                      Member, Ebonyi Diaspora
                    </p>
                  </div>
                </div>
              </div>
            </div>

            <!-- Contact Form -->
            <div class="lg:pl-12">
              <div class="overflow-hidden bg-gray-50 rounded-md shadow-md">
                <div class="p-6 sm:p-10">
                  <h3 class="text-3xl font-semibold text-green-600">
                    Contact Us
                  </h3>
                  <p class="mt-4 text-base text-gray-600">
                    Fill out the form below, and we’ll get back to you shortly.
                  </p>

                  <form action="#" method="POST" class="mt-4">
                    <div class="space-y-6">
                      <div>
                        <label
                          for="name"
                          class="text-base font-medium text-gray-900"
                          >Your Name</label
                        >
                        <div class="mt-2.5">
                          <input
                            type="text"
                            name="name"
                            id="name"
                            placeholder="Enter your full name"
                            class="block w-full px-4 py-4 text-gray-900 placeholder-gray-500 transition-all duration-200 bg-white border border-gray-200 rounded-md focus:outline-none focus:ring-green-500 focus:border-green-500"
                          />
                        </div>
                      </div>

                      <div>
                        <label
                          for="email"
                          class="text-base font-medium text-gray-900"
                          >Email Address</label
                        >
                        <div class="mt-2.5">
                          <input
                            type="email"
                            name="email"
                            id="email"
                            placeholder="Enter your email"
                            class="block w-full px-4 py-4 text-gray-900 placeholder-gray-500 transition-all duration-200 bg-white border border-gray-200 rounded-md focus:outline-none focus:ring-green-500 focus:border-green-500"
                          />
                        </div>
                      </div>

                      <div>
                        <label
                          for="message"
                          class="text-base font-medium text-gray-900"
                          >Message</label
                        >
                        <div class="mt-2.5">
                          <textarea
                            name="message"
                            id="message"
                            placeholder="Write your message here"
                            class="block w-full px-4 py-4 text-gray-900 placeholder-gray-500 transition-all duration-200 bg-white border border-gray-200 rounded-md resize-y focus:outline-none focus:ring-green-500 focus:border-green-500"
                            rows="4"
                          ></textarea>
                        </div>
                      </div>

                      <div>
                        <button
                          type="submit"
                          class="inline-flex items-center justify-center w-full px-4 py-4 text-base font-semibold text-white transition-all duration-200 bg-green-600 border border-transparent rounded-md hover:bg-green-700 focus:bg-green-700"
                        >
                          Send Message
                        </button>
                      </div>
                    </div>
                  </form>
                </div>
              </div>
            </div>

            <div class="md:hidden">
              <blockquote class="mt-6">
                <p class="text-lg leading-relaxed text-gray-600">
                  "Being part of this community has strengthened my connection
                  to home and created lifelong bonds."
                </p>
              </blockquote>
              <div class="flex items-center mt-8">
                <img
                  class="flex-shrink-0 object-cover w-10 h-10 rounded-full"
                  src="https://via.placeholder.com/150"
                  alt="Testimonial"
                />
                <div class="ml-4">
                  <p class="text-base font-semibold text-green-600">
                    Chidera Okonkwo
                  </p>
                  <p class="mt-px text-sm text-gray-500">
                    Member, Ebonyi Diaspora
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>
    </body>
  </html>
</template>

<!-- Add Tailwind CSS Keyframes -->
<style>
@keyframes fade-in-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }
  100% {
    opacity: 1;
    transform: translateY(0);
  }
}
.animate-fade-in-up {
  animation: fade-in-up 1s ease-out forwards;
}
</style>


