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
            <h3 class="text-4xl font-bold text-black">
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

          <form @submit.prevent="handleSubmit">
            <div class="space-y-5">
              <div>
                <label for="name" class="text-base font-medium text-gray-900">
                  Full Name
                </label>
                <input
                  type="text"
                  id="name"
                  v-model="form.name"
                  required
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
                  v-model="form.email"
                  required
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
                  v-model="form.phone"
                  required
                  placeholder="Enter your phone number (e.g., +123456789)"
                  class="block w-full mt-2.5 py-4 px-4 text-black placeholder-gray-500 border border-gray-200 rounded-md bg-gray-50 focus:outline-none focus:border-green-600 focus:bg-white caret-green-600"
                />
              </div>

              <div>
                <button
                  type="submit"
                  :disabled="loading"
                  class="inline-flex items-center justify-center w-full px-4 py-4 text-base font-semibold bg-white text-green-500 rounded-lg shadow border-2 border-green-500 hover:bg-green-500 hover:text-white transition-all duration-300"
                >
                  <span v-if="loading">Submitting...</span>
                  <span v-else>Join the Community</span>
                </button>
              </div>
              <div class="mt-4 flex space-x-2">
                <a
                  href="https://wa.me/your-group-link"
                  target="_blank"
                  class="flex-1 inline-flex items-center justify-center px-2 py-3 text-sm font-semibold text-white bg-green-500 rounded-md hover:bg-green-600 transition duration-200"
                >
                  <svg
                    class="w-4 h-4 mr-1"
                    xmlns="http://www.w3.org/2000/svg"
                    fill="currentColor"
                    viewBox="0 0 24 24"
                  >
                    <path
                      d="M12 0C5.372 0 0 5.373 0 12c0 2.118.55 4.108 1.514 5.844L0 24l6.272-1.594C8.096 23.461 10.016 24 12 24c6.627 0 12-5.373 12-12S18.627 0 12 0zm7.306 16.69l-1.924 1.917c-.438.436-1.002.671-1.59.666-1.523-.01-4.06-1.373-6.19-3.502-2.13-2.128-3.491-4.665-3.502-6.19-.005-.587.23-1.15.666-1.588l1.923-1.926c.43-.431 1.125-.431 1.556 0l1.396 1.396c.43.43.43 1.124 0 1.554L8.98 9.696c-.014.014-.019.034-.033.048.003.014.018.025.033.038 1.18 1.366 2.562 2.748 3.929 3.931.014.014.034.03.048.033.014-.014.034-.018.048-.033l1.491-1.488c.43-.43 1.124-.43 1.554 0l1.396 1.396c.432.431.432 1.124 0 1.556z"
                    />
                  </svg>
                  WhatsApp
                </a>

                <a
                  href="https://facebook.com/your-group-link"
                  target="_blank"
                  class="flex-1 inline-flex items-center justify-center px-2 py-3 text-sm font-semibold text-white bg-blue-600 rounded-md hover:bg-blue-700 transition duration-200"
                >
                  <svg
                    class="w-4 h-4 mr-1"
                    xmlns="http://www.w3.org/2000/svg"
                    fill="currentColor"
                    viewBox="0 0 24 24"
                  >
                    <path
                      d="M22.676 0H1.326C.594 0 0 .593 0 1.326v21.348C0 23.406.593 24 1.326 24h11.497v-9.294H9.847v-3.622h2.976v-2.687c0-2.938 1.797-4.548 4.42-4.548 1.256 0 2.339.093 2.654.135v3.074h-1.821c-1.43 0-1.706.678-1.706 1.673v2.354h3.413l-.445 3.622h-2.968V24h5.811c.733 0 1.326-.593 1.326-1.326V1.326C24 .594 23.407 0 22.676 0z"
                    />
                  </svg>
                  Facebook
                </a>
              </div>
            </div>
          </form>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
function doPost(e) {
  try {
    // Log incoming POST data for debugging
    Logger.log('Raw POST Data: ' + JSON.stringify(e));

    if (!e.postData) {
      throw new Error('No POST data received');
    }

    var data = JSON.parse(e.postData.contents);
    Logger.log('Parsed Data: ' + JSON.stringify(data));

    var sheet = SpreadsheetApp.getActiveSpreadsheet().getActiveSheet();
    sheet.appendRow([data.name, data.email, data.phone, new Date()]);

    // Return success response with proper CORS handling
    return ContentService.createTextOutput(JSON.stringify({ success: true }))
      .setMimeType(ContentService.MimeType.JSON)
    .setHeader("Access-Control-Allow-Origin", "https://www.ebonyidiaspora.com/");
  } catch (error) {
    Logger.log('Error: ' + error.message);

    return ContentService.createTextOutput(JSON.stringify({ success: false, error: error.message }))
      .setMimeType(ContentService.MimeType.JSON);
  }
}



function doGet(e) {
  return handleCORS();
}




function handleCORS() {
  const response = ContentService.createTextOutput();
  response.setMimeType(ContentService.MimeType.JSON);
  response.setContent('{"message":"CORS enabled"}');
  response.setHeader("Access-Control-Allow-Origin", "*");
  response.setHeader("Access-Control-Allow-Methods", "GET, POST, OPTIONS");
  response.setHeader("Access-Control-Allow-Headers", "Content-Type");
  return response;
}




export default {
  data() {
    return {
      form: {
        name: "",
        email: "",
        phone: "",
      },
      loading: false,
    };
  },
  methods: {
    async handleSubmit() {
      this.loading = true;
      try {
        const response = await fetch(
          "https://script.google.com/macros/s/AKfycbzi5jzsWc81vPt8ix6IlDkv6BqiUikJ_JhiAejMSpqgT5rSRQpy1z1t4Jm3NGZCops/exec",
          {
            method: "POST",
            headers: { "Content-Type": "application/json" },
            body: JSON.stringify({
              name: this.form.name,
              email: this.form.email,
              phone: this.form.phone,
            }),
          }
        );

        if (!response.ok) {
          throw new Error(`HTTP Error: ${response.status}`);
        }

        const result = await response.json();
        if (result.success) {
          alert("Form submitted successfully!");
        } else {
          alert("Submission failed: " + result.error);
        }
      } catch (error) {
        console.error("Error:", error);
        alert("Error: " + error.message);
      } finally {
        this.loading = false;
      }
    },
  },
};
</script>
