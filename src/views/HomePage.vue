<template>
  <router-link to="/accueil" class="min-h-screen flex items-center justify-center bg-gray-50">
    <div class="bg-white p-8 rounded-lg shadow-lg text-center sm:w-3/4 md:w-1/2 lg:w-1/3 xl:w-1/4">
      <h1 class="text-2xl font-bold mb-4">Gérez vos invités en toute sécurité</h1>

      <p class="mb-6">
        EventApp vous permet de gérer vos invités grâce à un système de Code QR universellement
        unique et sécurisé.
      </p>
      <img
        src="@/assets/img1.png"
        alt="World Map"
        class="mb-6 max-w-full h-auto transition-transform transform hover:scale-105"
      />
      <button
        @click.prevent="redirectToAccueil"
        class="bg-green-500 text-white px-6 py-2 rounded-full mb-4"
      >
        Commencer maintenant
      </button>
      <button class="bg-gray-200 text-gray-500 py-1 px-3 rounded-full">
        Événements, Lifestyle et expériences
      </button>
    </div>
  </router-link>
  <div>
    <BeakerIcon class="size-6 text-blue-500" />
  </div>
</template>

<script setup>
import { BeakerIcon } from '@heroicons/vue/24/solid'
import { useRouter } from 'vue-router'

const router = useRouter()

const redirectToAccueil = () => {
  router.push('/accueil')
}
</script>
