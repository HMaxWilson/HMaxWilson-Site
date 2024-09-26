<template>
  <footer class="bg-gray-300 dark:bg-gray-900 border-t border-gray-400 dark:border-gray-500 text-gray-800 dark:text-gray-200">
    <div class="container mx-auto py-4 px-4">
      <div class="flex flex-wrap items-center justify-between">
        <div class="flex flex-wrap mx-auto sm:mx-0 text-sm justify-around font-medium leading-5">
          <ul class="flex space-x-4">
            <router-link to="/" class="hover:text-blue-600 dark:hover:text-blue-400">Home</router-link>
            <router-link to="/about" class="hover:text-blue-600 dark:hover:text-blue-400">About</router-link>
          </ul>
        </div>

        <div class="hidden sm:block text-sm">
          Phone: <a href="tel:07562763552">07562 763 552</a> <br/>
          Email: <a href="mailto:H.MaxWilson@hotmail.com">H.MaxWilson@hotmail.com</a>
        </div>
      </div>
      <div class="text-center py-2">
        &copy; 2024 - HMaxWilson - All Rights Reserved
      </div>
    </div>
  </footer>
</template>