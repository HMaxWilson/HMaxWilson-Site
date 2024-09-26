<template>
  <div class="home">
    <ProfileSection class="relative z-[9999]" />

    <svg class="md:mt-[-80px] lg:mt-[-120px] scale-110" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
      <path class="fill-slate-500 dark:fill-gray-800" fill-opacity="1" d="M0,160L48,186.7C96,213,192,267,288,266.7C384,267,480,213,576,192C672,171,768,181,864,186.7C960,192,1056,192,1152,186.7C1248,181,1344,171,1392,165.3L1440,160L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"></path>
    </svg>

    <ProjectsSection class="bg-slate-500 dark:bg-gray-800" />
  </div>
</template>

<script setup>
  import ProfileSection from "@/components/global/Pages/Home/ProfileSection.vue";
  import ProjectsSection from "@/components/global/Pages/Home/ProjectsSection.vue";
</script>
