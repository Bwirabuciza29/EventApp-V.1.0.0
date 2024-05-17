<template>
  <nav class="text-black">
    <div class="container mx-auto flex items-center justify-between p-2">
      <h4 data-aos="fade-up" class="text-xl font-bold">Événements à venir</h4>
      <div class="flex items-center">
        <div data-aos="fade-right" class="text-sm text-gray bold">Voir plus</div>
      </div>
    </div>
  </nav>

  <div class="flex justify-center items-center px-4 pb-4 overflow-x-auto scrollbar-smooth">
    <div
      class="flex justify-center items-center px-4 pb-4 gap-1 mx-auto overflow-x-auto scrollbar-smooth"
    >
      <div data-aos="fade-up" class="max-w-sm w-3/4 mx-auto" @click="redirectToAbout">
        <!-- Réduire la largeur de la div -->
        <div class="bg-white shadow-md rounded-lg overflow-hidden">
          <div class="relative">
            <img
              class="w-full h-48 object-cover object-center"
              src="../assets/iiii.jpg"
              alt="Image"
            />
            <!-- Réduire la hauteur de l'image -->
            <div class="absolute inset-0 flex items-center justify-center">
              <!-- Icône à gauche -->
              <div class="absolute left-2 top-2 p-2 bg-gray-800 rounded-lg">
                <div
                  class="event-card px-2 bg-gray-800 text-white rounded-lg px flex flex-col items-center"
                >
                  <div class="text-xl font-semibold mb-2 flex-grow">26</div>
                  <p class="text-sm flex-grow">Mai</p>
                </div>
              </div>
              <!-- Icônes à droite -->
              <div class="absolute right-0 top-0 flex space-x-2 p-2">
                <div
                  class="h-4 w-4 sm:h-6 sm:w-6 flex justify-center items-center rounded-full bg-gray-200"
                >
                  <!-- Réduire la taille des icônes -->
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke-width="1.5"
                    stroke="currentColor"
                    class="w-4 h-4 mr-1 text-gray-600 px"
                  >
                    <!-- Réduire la taille des icônes -->
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      d="M21 8.25c0-2.485-2.099-4.5-4.688-4.5-1.935 0-3.597 1.126-4.312 2.733-.715-1.607-2.377-2.733-4.313-2.733C5.1 3.75 3 5.765 3 8.25c0 7.22 9 12 9 12s9-4.78 9-12Z"
                    />
                  </svg>
                </div>
                <div
                  class="h-4 w-4 sm:h-6 sm:w-6 flex justify-center items-center rounded-full bg-gray-200"
                >
                  <!-- Réduire la taille des icônes -->
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke-width="1.5"
                    stroke="currentColor"
                    class="w-4 h-4 mr-1 text-gray-600"
                  >
                    <!-- Réduire la taille des icônes -->
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      d="M9 8.25H7.5a2.25 2.25 0 0 0-2.25 2.25v9a2.25 2.25 0 0 0 2.25 2.25h9a2.25 2.25 0 0 0 2.25-2.25v-9a2.25 2.25 0 0 0-2.25-2.25H15m0-3-3-3m0 0-3 3m3-3V15"
                    />
                  </svg>
                </div>
              </div>
            </div>
          </div>

          <div class="p-1">
            <h3 class="text-black text-lg font-bold">
              Lancement officiel : Congo Telement Event 2024
            </h3>
            <div class="bg-gray-100">
              <div class="max-w-md p-2 bg-white">
                <!-- Réduire le padding -->
                <p class="text-blue-600 text-left my-1">26 Mai 2024, 09:00</p>
                <div class="flex items-center mb-2">
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    class="w-4 h-4 mr-1 text-gray-600"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke="currentColor"
                  >
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      d="M15 10.5a3 3 0 1 1-6 0 3 3 0 0 1 6 0Z"
                    />
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      d="M19.5 10.5c0 7.142-7.5 11.25-7.5 11.25S4.5 17.642 4.5 10.5a7.5 7.5 0 1 1 15 0Z"
                    />
                  </svg>
                  <p class="text-gray-600 text-xs">Kinshasa, Gombe N23</p>
                  <!-- Réduire la taille de la police -->
                </div>
                <div class="mx-auto flex items-center justify-between p-1">
                  <p class="bg-blue-500/5 text-xs text-gray-500 py-0.5 px-2 rounded-full font-bold">
                    <!-- Réduire la taille de la police et du padding -->
                    Evenement physique
                  </p>
                  <div class="flex space-x-1 items-center">
                    <!-- Réduire l'espace entre les éléments -->
                    <span
                      class="cursor-pointer rounded-full border-gray-900/5 bg-blue-500/5 p-2 text-gray-900 transition-colors hover:border-gray-900/10 hover:bg-gray-900/10 hover:!opacity-100 group-hover:opacity-70"
                    >
                      <svg
                        xmlns="http://www.w3.org/2000/svg"
                        fill="none"
                        viewBox="0 0 24 24"
                        stroke-width="1.5"
                        stroke="currentColor"
                        class="w-4 h-4 text-gray"
                      >
                        <path
                          stroke-linecap="round"
                          stroke-linejoin="round"
                          d="M3 16.5v2.25A2.25 2.25 0 0 0 5.25 21h13.5A2.25 2.25 0 0 0 21 18.75V16.5m-13.5-9L12 3m0 0 4.5 4.5M12 3v13.5"
                        />
                      </svg>
                    </span>
                    <span
                      class="cursor-pointer rounded-full border-gray-900/5 bg-blue-400/5 p-2 text-gray-900 transition-colors hover:border-gray-900/10 hover:bg-gray-900/10 hover:!opacity-100 group-hover:opacity-70"
                    >
                      <svg
                        xmlns="http://www.w3.org/2000/svg"
                        fill="none"
                        viewBox="0 0 24 24"
                        stroke-width="1.5"
                        stroke="currentColor"
                        class="w-4 h-4 text-gray"
                      >
                        <path
                          stroke-linecap="round"
                          stroke-linejoin="round"
                          d="M16.5 3.75V16.5L12 14.25 7.5 16.5V3.75m9 0H18A2.25 2.25 0 0 1 20.25 6v12A2.25 2.25 0 0 1 18 20.25H6A2.25 2.25 0 0 1 3.75 18V6A2.25 2.25 0 0 1 6 3.75h1.5m9 0h-9"
                        />
                      </svg>
                    </span>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div data-aos="fade-up" class="max-w-sm w-3/4 mx-auto" @click="redirectToAbout">
        <!-- Réduire la largeur de la div -->
        <div class="bg-white shadow-md rounded-lg overflow-hidden">
          <div class="relative">
            <img
              class="w-full h-48 object-cover object-center"
              src="../assets/iiii.jpg"
              alt="Image"
            />
            <!-- Réduire la hauteur de l'image -->
            <div class="absolute inset-0 flex items-center justify-center">
              <!-- Icône à gauche -->
              <div class="absolute left-2 top-2 p-2 bg-gray-800 rounded-lg">
                <div
                  class="event-card px-2 bg-gray-800 text-white rounded-lg px flex flex-col items-center"
                >
                  <div class="text-xl font-semibold mb-2 flex-grow">26</div>
                  <p class="text-sm flex-grow">Mai</p>
                </div>
              </div>
              <!-- Icônes à droite -->
              <div class="absolute right-0 top-0 flex space-x-2 p-2">
                <div
                  class="h-4 w-4 sm:h-6 sm:w-6 flex justify-center items-center rounded-full bg-gray-200"
                >
                  <!-- Réduire la taille des icônes -->
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke-width="1.5"
                    stroke="currentColor"
                    class="w-4 h-4 mr-1 text-gray-600 px"
                  >
                    <!-- Réduire la taille des icônes -->
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      d="M21 8.25c0-2.485-2.099-4.5-4.688-4.5-1.935 0-3.597 1.126-4.312 2.733-.715-1.607-2.377-2.733-4.313-2.733C5.1 3.75 3 5.765 3 8.25c0 7.22 9 12 9 12s9-4.78 9-12Z"
                    />
                  </svg>
                </div>
                <div
                  class="h-4 w-4 sm:h-6 sm:w-6 flex justify-center items-center rounded-full bg-gray-200"
                >
                  <!-- Réduire la taille des icônes -->
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke-width="1.5"
                    stroke="currentColor"
                    class="w-4 h-4 mr-1 text-gray-600"
                  >
                    <!-- Réduire la taille des icônes -->
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      d="M9 8.25H7.5a2.25 2.25 0 0 0-2.25 2.25v9a2.25 2.25 0 0 0 2.25 2.25h9a2.25 2.25 0 0 0 2.25-2.25v-9a2.25 2.25 0 0 0-2.25-2.25H15m0-3-3-3m0 0-3 3m3-3V15"
                    />
                  </svg>
                </div>
              </div>
            </div>
          </div>

          <div class="p-1">
            <h3 class="text-black text-lg font-bold">
              Lancement officiel : Congo Telement Event 2024
            </h3>
            <div class="bg-gray-100">
              <div class="max-w-md p-2 bg-white">
                <!-- Réduire le padding -->
                <p class="text-blue-600 text-left my-1">26 Mai 2024, 09:00</p>
                <div class="flex items-center mb-2">
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    class="w-4 h-4 mr-1 text-gray-600"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke="currentColor"
                  >
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      d="M15 10.5a3 3 0 1 1-6 0 3 3 0 0 1 6 0Z"
                    />
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      d="M19.5 10.5c0 7.142-7.5 11.25-7.5 11.25S4.5 17.642 4.5 10.5a7.5 7.5 0 1 1 15 0Z"
                    />
                  </svg>
                  <p class="text-gray-600 text-xs">Kinshasa, Gombe N23</p>
                  <!-- Réduire la taille de la police -->
                </div>
                <div class="mx-auto flex items-center justify-between p-1">
                  <p class="bg-blue-500/5 text-xs text-gray-500 py-0.5 px-2 rounded-full font-bold">
                    <!-- Réduire la taille de la police et du padding -->
                    Evenement physique
                  </p>
                  <div class="flex space-x-1 items-center">
                    <!-- Réduire l'espace entre les éléments -->
                    <span
                      class="cursor-pointer rounded-full border-gray-900/5 bg-blue-500/5 p-2 text-gray-900 transition-colors hover:border-gray-900/10 hover:bg-gray-900/10 hover:!opacity-100 group-hover:opacity-70"
                    >
                      <svg
                        xmlns="http://www.w3.org/2000/svg"
                        fill="none"
                        viewBox="0 0 24 24"
                        stroke-width="1.5"
                        stroke="currentColor"
                        class="w-4 h-4 text-gray"
                      >
                        <path
                          stroke-linecap="round"
                          stroke-linejoin="round"
                          d="M3 16.5v2.25A2.25 2.25 0 0 0 5.25 21h13.5A2.25 2.25 0 0 0 21 18.75V16.5m-13.5-9L12 3m0 0 4.5 4.5M12 3v13.5"
                        />
                      </svg>
                    </span>
                    <span
                      class="cursor-pointer rounded-full border-gray-900/5 bg-blue-400/5 p-2 text-gray-900 transition-colors hover:border-gray-900/10 hover:bg-gray-900/10 hover:!opacity-100 group-hover:opacity-70"
                    >
                      <svg
                        xmlns="http://www.w3.org/2000/svg"
                        fill="none"
                        viewBox="0 0 24 24"
                        stroke-width="1.5"
                        stroke="currentColor"
                        class="w-4 h-4 text-gray"
                      >
                        <path
                          stroke-linecap="round"
                          stroke-linejoin="round"
                          d="M16.5 3.75V16.5L12 14.25 7.5 16.5V3.75m9 0H18A2.25 2.25 0 0 1 20.25 6v12A2.25 2.25 0 0 1 18 20.25H6A2.25 2.25 0 0 1 3.75 18V6A2.25 2.25 0 0 1 6 3.75h1.5m9 0h-9"
                        />
                      </svg>
                    </span>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import { defineComponent } from 'vue'
import AOS from 'aos'
import 'aos/dist/aos.css'

export default defineComponent({
  methods: {
    redirectToAbout() {
      // Rediriger vers la route "/about"
      this.$router.push('/about')
    }
  },
  mounted() {
    AOS.init()
  }
})
</script>
