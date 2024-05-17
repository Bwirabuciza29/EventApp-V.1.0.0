<template>
  <div class="min-h-screen flex flex-col items-center justify-center bg-gray-50">
    <div
      class="bg-white p-4 mt-4 rounded-lg shadow-lg text-center sm:w-5/6 md:w-3/4 lg:w-2/3 xl:w-1/2 mb-2"
    >
      <AccueilComp />
    </div>
    <div
      class="bg-white p-4 mt-2 rounded-lg shadow-lg text-center sm:w-5/6 md:w-3/4 lg:w-2/3 xl:w-1/2"
    >
      <ComingEvents />
    </div>
    <div
      class="bg-white m-2 my px-4 rounded-lg shadow-lg text-center sm:w-5/6 md:w-3/4 lg:w-2/3 xl:w-1/2"
    >
      <PassedEvents />
    </div>
    <div
      class="mt-2 mb-2 my px-4 rounded-full shadow-lg text-center items-center sm:w-5/6 md:w-3/4 lg:w-2/3 xl:w-1/2"
    >
      <footer class="py-4 text-center">
        <div
          class="bg-white p-3 rounded-full pl-auto border pr-auto inline-flex flex-wrap items-center justify-center gap-3 mt-8 group sm:w-5/6 md:w-3/4 lg:w-2/3 xl:w-1/2 w-full"
        >
          <span
            v-for="(icon, index) in icons"
            :key="index"
            :class="iconClass(index)"
            @click="setActiveIcon(index)"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke-width="1.5"
              stroke="currentColor"
              class="w-6 h-6"
            >
              <path :d="icon.path" stroke-linecap="round" stroke-linejoin="round" />
            </svg>
          </span>
        </div>
      </footer>
    </div>
  </div>
</template>
<script setup>
import { ref } from 'vue'

// Import du composant AccueilComp
import AccueilComp from '../components/AccueilComp.vue'
import ComingEvents from '../components/ComingEvents.vue'
import PassedEvents from '../components/PassedEvents.vue'

const icons = ref([
  {
    path: 'M2.25 12L11.204 3.045c.44-.439 1.152-.439 1.591 0L21.75 12M4.5 9.75v10.125c0 .621.504 1.125 1.125 1.125H9.75v-4.875c0-.621.504-1.125 1.125-1.125h2.25c.621 0 1.125.504 1.125 1.125V21h4.125c.621 0 1.125-.504 1.125-1.125V9.75M8.25 21h8.25'
  },
  {
    path: 'M6.75 3v2.25M17.25 3v2.25M3 18.75V7.5a2.25 2.25 0 0 1 2.25-2.25h13.5A2.25 2.25 0 0 1 21 7.5v11.25m-18 0A2.25 2.25 0 0 0 5.25 21h13.5A2.25 2.25 0 0 0 21 18.75m-18 0v-7.5A2.25 2.25 0 0 1 5.25 9h13.5A2.25 2.25 0 0 1 21 11.25v7.5m-9-6h.008v.008H12v-.008ZM12 15h.008v.008H12V15Zm0 2.25h.008v.008H12v-.008ZM9.75 15h.008v.008H9.75V15Zm0 2.25h.008v.008H9.75v-.008ZM7.5 15h.008v.008H7.5V15Zm0 2.25h.008v.008H7.5v-.008Zm6.75-4.5h.008v.008h-.008v-.008Zm0 2.25h.008v.008h-.008V15Zm0 2.25h.008v.008h-.008v-.008Zm2.25-4.5h.008v.008H16.5v-.008Zm0 2.25h.008v.008H16.5V15Z'
  },
  {
    path: 'M15.75 6a3.75 3.75 0 1 1-7.5 0 3.75 3.75 0 0 1 7.5 0ZM4.501 20.118a7.5 7.5 0 0 1 14.998 0A17.933 17.933 0 0 1 12 21.75c-2.676 0-5.216-.584-7.499-1.632Z'
  }
])

const activeIndex = ref(0)

const setActiveIcon = (index) => {
  activeIndex.value = index
}

const iconClass = (index) => {
  return {
    'rounded-full p-3 transition-colors': true,
    'border border-gray-900/5 bg-black text-white': activeIndex.value === index,
    'border border-gray-900/5 bg-gray-900/5 text-gray-900': activeIndex.value !== index
  }
}
</script>
<style>
footer {
  position: fixed;
  left: 0;
  bottom: 0;
  width: 100%;
  padding: 1rem;
  z-index: 999;
}
</style>