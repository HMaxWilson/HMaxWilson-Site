<template>
  <img src="@/assets/HMaxWilson.webp" alt="Profile Picture of Harrison Max Wilson"
       class="w-full border-2 border-blue-800 dark:border-blue-400 scale-90 hover:scale-100"/>
</template>

<script setup>

</script>

<style scoped>
  img {
    -webkit-animation: morph 8s ease-in-out infinite;
    animation: morph 8s ease-in-out infinite;
    border-radius: 60% 40% 30% 70% / 60% 30% 70% 40%;
    transition: all 1s ease-in-out;
  }

  @keyframes morph {
    0%, 100% {
      border-radius: 60% 40% 30% 70% / 60% 30% 70% 40%;
    }
    50% {
      border-radius: 30% 60% 70% 40% / 50% 60% 40% 70%;
    }
  }
</style>