<script setup>
import { RouterView } from 'vue-router'
import Header from './components/global/TheHeader.vue'
import Footer from './components/global/TheFooter.vue'
</script>

<template>
  <Header />

  <main class="container mx-auto pt-10 px-12 text-black text-center">
    <RouterView />
  </main>

  <Footer />
</template>
