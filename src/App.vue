<template>
  <Header />

  <main>
    <RouterView />
  </main>

  <Footer />
</template>

<script setup>
  import { RouterView } from 'vue-router'
  import Header from '@/components/global/Header/TheHeader.vue'
  import Footer from '@/components/global/Footer/TheFooter.vue'
</script>