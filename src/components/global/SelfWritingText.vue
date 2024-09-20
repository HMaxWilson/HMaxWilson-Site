<template>
  <span class="text-2xl sm:text-4xl font-bold space-x-2 text-blue-800 dark:text-blue-400">
    {{ typingEffect }}
    <span class="animate-pulse text-3xl sm:text-5xl">|</span>
  </span>
</template>

<script setup>
import { onMounted, ref } from "vue";

const props = defineProps({
  words: Array
})

const typingEffect = ref('')
let wordIndex = 0;

onMounted(() => {
  let i = 0;
  let isDeleting = false;

  const typeWriter = () => {
    const currentWord = props.words[wordIndex];

    if (!isDeleting) {
      typingEffect.value = currentWord.substring(0, i + 1);
      i++;

      if (i === currentWord.length) {
        setTimeout(() => {
          isDeleting = true;
        }, 1000);
      }
    } else {
      typingEffect.value = currentWord.substring(0, i - 1);
      i--;

      if (i === 0) {
        isDeleting = false;
        wordIndex = (wordIndex + 1) % props.words.length;
      }
    }

    const speed = isDeleting
        ? Math.floor(Math.random() * (80 - 30 + 1)) + 30
        : Math.floor(Math.random() * (150 - 50 + 1)) + 50;

    setTimeout(typeWriter, speed);
  }

  typeWriter();
})
</script>
