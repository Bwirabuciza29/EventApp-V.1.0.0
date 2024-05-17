<template>
  <div class="min-h-screen flex flex-col items-center justify-center bg-gray-50">
    <div
      class="bg-[url('src/assets/iiii.jpg')] p-4 mt-4 shadow-lg text-center sm:w-5/6 md:w-3/4 lg:w-2/3 xl:w-1/2 mb-2 bg-cover bg-center min-h-40"
    >
      <EventsDetails />
    </div>
    <div
      class="bg-white p-4 shadow-lg text-center sm:w-5/6 md:w-3/4 lg:w-2/3 xl:w-1/2 mb-2 bg-cover bg-center"
    >
      <DetailOne />
    </div>
    <div
      class="bg-white p-4 shadow-lg text-center sm:w-5/6 md:w-3/4 lg:w-2/3 xl:w-1/2 mb-2 bg-cover bg-center"
    >
      <DetailSecond />
    </div>
  </div>
</template>
<script setup>
// Import du composant AccueilComp
import EventsDetails from '../components/EventsDetails/EventsDetails.vue'
import DetailOne from '../components/EventsDetails/DetailOne.vue'
import DetailSecond from '../components/EventsDetails/DetailSecond.vue'
</script>