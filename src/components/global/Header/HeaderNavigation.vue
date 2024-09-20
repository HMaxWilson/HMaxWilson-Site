<template>
  <nav>
    <ul class="flex space-x-6 text-sm font-medium leading-5">
      <li v-for="item in navigation" :key="item.name">
        <RouterLink :to="item.link" class="hover:text-gray-700">{{ item.name }}</RouterLink>
      </li>
    </ul>
  </nav>
</template>

<script setup>

const navigation = [
  // {
  //   name: 'Home',
  //   link: '/'
  // },
  // {
  //   name: 'About',
  //   link: '/about'
  // }
]
</script>
