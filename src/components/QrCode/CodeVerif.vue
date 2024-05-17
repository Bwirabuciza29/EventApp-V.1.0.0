<template>
  <div class="min-h-screen flex flex-col items-center justify-center bg-gray-50">
    <div
      class="bg-white p-4 mt-4 rounded-lg shadow-lg text-center sm:w-5/6 md:w-3/4 lg:w-2/3 xl:w-1/2 mb-2"
    >
      <nav data-aos="fade-up" class="text-black">
        <div class="container mx-auto flex items-center justify-between p-2">
          <div
            class="h-6 w-6 sm:h-8 sm:w-8 flex justify-center items-center rounded-full bg-gray-200"
          >
            <svg
              @click.prevent="redirectToHOme"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke-width="1.5"
              stroke="currentColor"
              class="w-4 h-4 sm:w-6 sm:h-6"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                d="M6.75 15.75 3 12m0 0 3.75-3.75M3 12h18"
              />
            </svg>
          </div>
          <div class="flex space-x-2 items-center">
            <h1 class="text-xl sm:text-2xl font-bold">Scanner le code</h1>
          </div>
        </div>

        <div class="flex justify-center items-center">
          <div class="qr-container relative w-72 h-72 bg-white border-2 border-gray-300">
            <vue-qrious :value="JSON.stringify(Mytext)" size="300" />
          </div>
          <div class="qr-scanner absolute bottom-0 left-0 w-full h-2 bg-gray-500">
            <button
              @click="exitScanner"
              class="qr-button absolute bottom-4 left-1/2 transform -translate-x-1/2 bg-gray-700 text-white px-8 py-2 rounded-full cursor-pointer"
            >
              Quitter
            </button>
          </div>
        </div>
      </nav>
    </div>
  </div>
</template>
<script>
import { defineComponent } from 'vue'
import AOS from 'aos'
import 'aos/dist/aos.css'
import VueQrious from 'vue-qrious'

export default defineComponent({
  setup() {},
  mounted() {
    AOS.init()
  }
})
</script>
<script setup>
import { useRouter } from 'vue-router'

const router = useRouter()

const redirectToHOme = () => {
  router.push('/accueil')
}
</script>
