<template>
    <section class="h-[100vh] w-full bg-white">
        <div class="flex lg:flex-row flex-col gap-4 h-full">

            <!-- Hero Content -->
            <div class="flex-1 flex items-center justify-center">
                <div class="p-6 pt-12 lg:p-12">
                    <h1 class="text-3xl lg:text-5xl font-bold text-surface-900 dark:text-surface-0 mb-4 lg:leading-normal text-center lg:text-left">
                        Celebrating Ebonyi Heritage in <span class="text-green-500 dark:text-green-400">Kenya's Diaspora</span>
                    </h1>
                    <p class="text-surface-700 dark:text-surface-200 leading-normal mb-8 text-center lg:text-left">
                        Connect, network, and celebrate the rich culture of Ebonyi indigenes in Kenya. Join our community to stay informed and involved.
                    </p>
                    <div class="flex items-center justify-center lg:justify-start gap-6">
  <a 
    href="/join" 
    class="px-6 py-3 bg-green-500 text-white font-bold rounded-lg shadow hover:bg-green-600 transition-all duration-300"
  >
    Join the Community
  </a>
  <a 
    href="/event" 
    class="px-6 py-3 bg-white text-green-500 font-bold rounded-lg shadow border-2 border-green-500 hover:bg-green-500 hover:text-white transition-all duration-300"
  >
    Explore Events
  </a>
</div>

                </div>
            </div>

            <!-- Hero Video -->
            <div class="flex-1 overflow-hidden relative">
                <video
                    class="h-full w-full object-cover lg:[clip-path:polygon(12%_0,100%_0%,100%_100%,0_100%)]"
                    playsinline
                    autoplay
                    muted
                    loop
                >
                    <source src="/assets/videos/flag.mp4" type="video/mp4" />
                    Your browser does not support the video tag.
                </video>
            </div>

        </div>
    </section>
</template>

<style scoped>

</style>
