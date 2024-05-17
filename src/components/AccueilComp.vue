<template>
  <nav data-aos="fade-up" class="text-black">
    <div class="container mx-auto flex items-center justify-between p-2">
      <h1 class="text-xl sm:text-2xl font-bold">Accueil</h1>
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
            class="w-4 h-4 sm:w-6 sm:h-6"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M14.857 17.082a23.848 23.848 0 0 0 5.454-1.31A8.967 8.967 0 0 1 18 9.75V9A6 6 0 0 0 6 9v.75a8.967 8.967 0 0 1-2.312 6.022c1.733.64 3.56 1.085 5.455 1.31m5.714 0a24.255 24.255 0 0 1-5.714 0m5.714 0a3 3 0 1 1-5.714 0"
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
            class="w-4 h-4 sm:w-6 sm:h-6"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M6.75 3v2.25M17.25 3v2.25M3 18.75V7.5a2.25 2.25 0 0 1 2.25-2.25h13.5A2.25 2.25 0 0 1 21 7.5v11.25m-18 0A2.25 2.25 0 0 0 5.25 21h13.5A2.25 2.25 0 0 0 21 18.75m-18 0v-7.5A2.25 2.25 0 0 1 5.25 9h13.5A2.25 2.25 0 0 1 21 11.25v7.5m-9-6h.008v.008H12v-.008ZM12 15h.008v.008H12V15Zm0 2.25h.008v.008H12v-.008ZM9.75 15h.008v.008H9.75V15Zm0 2.25h.008v.008H9.75v-.008ZM7.5 15h.008v.008H7.5V15Zm0 2.25h.008v.008H7.5v-.008Zm6.75-4.5h.008v.008h-.008v-.008Zm0 2.25h.008v.008h-.008V15Zm0 2.25h.008v.008h-.008v-.008Zm2.25-4.5h.008v.008H16.5v-.008Zm0 2.25h.008v.008H16.5V15Z"
            />
          </svg>
        </div>
      </div>
    </div>
    <div class="flex flex-col sm:flex-row space-y-2 sm:space-y-0 sm:space-x-2">
      <button
        v-for="(button, index) in buttons"
        :key="index"
        :class="buttonClass(index)"
        @click="setActiveButton(index)"
      >
        {{ button.label }}
      </button>
    </div>
  </nav>
</template>
<script>
import { ref } from 'vue'
import { defineComponent } from 'vue'
import AOS from 'aos'
import 'aos/dist/aos.css'

export default defineComponent({
  setup() {
    const buttons = ref([
      { label: 'Parcourir' },
      { label: 'Événements' },
      { label: 'Statistiques' }
    ])

    const activeIndex = ref(0)

    const setActiveButton = (index) => {
      activeIndex.value = index
    }

    const buttonClass = (index) => {
      return {
        'bg-black text-white': activeIndex.value === index,
        'bg-gray-100 text-gray-800 border border-gray-300': activeIndex.value !== index,
        'px-2 py-1 rounded-full sm:px-4 sm:py-2': index === 0,
        'px-1 py-1 rounded-full sm:px-2 sm:py-2': index !== 0
      }
    }

    return {
      buttons,
      activeIndex,
      setActiveButton,
      buttonClass
    }
  },
  mounted() {
    AOS.init()
  }
})
</script>
