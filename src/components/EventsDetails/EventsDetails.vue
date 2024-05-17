<template>
  <nav data-aos="fade-up" class="text-black">
    <div data-aos="fade-up" class="container mx-auto flex items-center justify-between p-2">
      <div class="h-6 w-6 sm:h-8 sm:w-8 flex justify-center items-center rounded-full bg-gray-200">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 24 24"
          stroke-width="1.5"
          stroke="currentColor"
          @click="redirectToAccueil"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M10.5 19.5 3 12m0 0 7.5-7.5M3 12h18"
          />
        </svg>
      </div>
      <div class="flex space-x-2 items-center">
        <!-- Ajout de l'icône pour les notifications -->
        <div
          class="h-6 w-6 sm:h-8 sm:w-8 flex justify-center items-center rounded-full bg-gray-200"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="currentColor"
            class="w-6 h-6"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M3 16.5v2.25A2.25 2.25 0 0 0 5.25 21h13.5A2.25 2.25 0 0 0 21 18.75V16.5m-13.5-9L12 3m0 0 4.5 4.5M12 3v13.5"
            />
          </svg>
        </div>
        <div
          class="h-6 w-6 sm:h-8 sm:w-8 flex justify-center items-center rounded-full bg-gray-200"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="currentColor"
            class="w-6 h-6"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M21 8.25c0-2.485-2.099-4.5-4.688-4.5-1.935 0-3.597 1.126-4.312 2.733-.715-1.607-2.377-2.733-4.313-2.733C5.1 3.75 3 5.765 3 8.25c0 7.22 9 12 9 12s9-4.78 9-12Z"
            />
          </svg>
        </div>
      </div>
    </div>
    <div class="flex flex-col sm:flex-row space-y-2 sm:space-y-0 sm:space-x-2"></div>
  </nav>
</template>
<script>
import { defineComponent } from 'vue'
import AOS from 'aos'
import 'aos/dist/aos.css'

export default defineComponent({
  methods: {
    redirectToAccueil() {
      // Rediriger vers la route "/about"
      this.$router.push('/accueil')
    }
  },
  mounted() {
    AOS.init()
  }
})
</script>