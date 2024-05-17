<script setup>
import { RouterView } from 'vue-router'
</script>
<template>
  <RouterView />
</template>
<script>
import { defineComponent } from 'vue'
import AOS from 'aos'
import 'aos/dist/aos.css'

export default defineComponent({
  mounted() {
    AOS.init()
    this.$router.push('/loading')
  }
})
</script>