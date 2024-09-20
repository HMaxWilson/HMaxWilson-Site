<template>
  <header class="bg-gray-200 dark:bg-gray-800 border-b border-gray-300 dark:border-gray-500 shadow-md">
    <div class="container mx-auto p-4">
      <div class="flex justify-between">
        <div class="flex space-x-4 items-center">
          <ThemeToggle />

          <HeaderLogo />
        </div>

        <HeaderNavigation />
      </div>
    </div>
  </header>
</template>

<script setup>
  import ThemeToggle from '@/components/global/header/ThemeToggle.vue'
  import HeaderLogo from '@/components/global/header/HeaderLogo.vue'
  import HeaderNavigation from '@/components/global/header/HeaderNavigation.vue'
</script>