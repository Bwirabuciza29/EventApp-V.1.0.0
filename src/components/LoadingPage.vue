<!-- ./src/components/LoadingPage.vue -->
<template>
  <div class="flex items-center justify-center min-h-screen bg-gray-100">
    <div class="text-center">
      <div
        class="loader ease-linear rounded-full border-8 border-t-8 border-gray-200 h-64 w-64 mb-4"
      ></div>
      <h2 class="text-xl font-semibold">Chargement...</h2>
      <p class="text-gray-500">Veuillez patienter.</p>
    </div>
  </div>
</template>

<script>
export default {
  mounted() {
    setTimeout(() => {
      this.$router.push('/')
    }, 3000) // Redirige après 3 secondes
  }
}
</script>

<style>
.loader {
  border-top-color: #3498db;
  animation: spin 1s infinite linear;
}

@keyframes spin {
  to {
    transform: rotate(360deg);
  }
}
</style>
