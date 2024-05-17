<template>
  <div class="min-h-screen flex flex-col items-center justify-center bg-gray-50">
    <div
      class="bg-white p-4 mt-4 rounded-lg shadow-lg text-center sm:w-5/6 md:w-3/4 lg:w-2/3 xl:w-1/2 mb-2"
    >
      <GuestsComp />
    </div>
    <div
      class="bg-white p-4 mt-4 rounded-lg shadow-lg text-center sm:w-5/6 md:w-3/4 lg:w-2/3 xl:w-1/2 mb-2"
    >
      <GuestsSearch />
    </div>
  </div>
</template>
<script setup>
// Import du composant AccueilComp
import GuestsComp from '../components/Guests/GuestsComp.vue'
import GuestsSearch from '../components/Guests/GuestsSearch.vue'
</script>
