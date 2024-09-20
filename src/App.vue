<template>
  <Header />

  <main class="container mx-auto p-8">
    <RouterView />
  </main>

  <Footer />
</template>

<script setup>
  import { RouterView } from 'vue-router'
  import Header from '@/components/global/Header/TheHeader.vue'
  import Footer from '@/components/global/Footer/TheFooter.vue'
</script>