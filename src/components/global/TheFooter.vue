<template>
  <footer class="bg-black border-t border-gray-500 text-gray-400">
    <div class="container mx-auto py-4 px-4">
      <div class="flex flex-wrap items-center justify-between">
        <div class="flex flex-wrap mx-auto sm:mx-0 text-sm justify-around font-medium leading-5">
          <RouterLink to="/" class="px-3 py-1 hover:font-bold">Home</RouterLink>
          <RouterLink to="/about" class="px-3 py-1 hover:font-bold">About</RouterLink>
        </div>
        <div class="hidden sm:block text-sm">
          Phone: <a class="opacity-80 hover:opacity-100" href="tel:"></a> <br/>
          Email: <a class="opacity-80 hover:opacity-100" href="mailto:"></a>
        </div>
      </div>
      <div class="text-center py-2">
        &copy; Template
      </div>
    </div>
  </footer>
</template>

<script setup>
import { RouterLink } from 'vue-router'
</script>