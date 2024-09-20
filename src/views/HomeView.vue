<template>
  <div>
    <div id="Profile" class="flex-col space-y-4">
      <div class="flex flex-col-reverse md:flex-row gap-4">
        <div class="w-full sm:w-2/3 space-y-4">
          <div class="flex flex-col text-2xl md:text-3xl">
            <span>Hi, I'm <b>Harrison</b></span>
            <span>Your <SelfWritingText :words="words" /> Developer</span>
          </div>

          <div class="text-xl space-y-8">
            <p>I'm a Full Stack Developer with a passion for creating charming and functional websites.</p>

            <p>More info coming soon...</p>
          </div>
        </div>

        <div class="flex-1">
          <AvatarImage />
        </div>
      </div>

      <div id="Skills">
        <div class="flex flex-col md:flex-row items-center md:space-x-4">
          <p class="text-2xl font-bold md:border-r-2 border-black md:pr-4 mb-2 md:mb-0">Tech Stack</p>

          <ul class="flex flex-col md:flex-row space-y-4 md:space-y-0 md:space-x-8 items-center">
            <li class="hover:scale-110 transform transition duration-300">
              <img src="https://skillicons.dev/icons?i=html" title="HTML" alt="HTML skill-icon">
            </li>
            <li class="hover:scale-110 transform transition duration-300">
              <img src="https://skillicons.dev/icons?i=css,tailwind" title="CSS & Tailwind" alt="CSS/Tailwind skill-icon">
            </li>
            <li class="hover:scale-110 transform transition duration-300">
              <img src="https://skillicons.dev/icons?i=js,vue,react" title="JavaScript, Vue & React" alt="JavaScript/Vue/React skill-icon">
            </li>
            <li class="hover:scale-110 transform transition duration-300">
              <img src="https://skillicons.dev/icons?i=php,laravel" title="PHP & Laravel" alt="PHP/Laravel skill-icon">
            </li>
            <li class="hover:scale-110 transform transition duration-300">
              <img src="https://skillicons.dev/icons?i=postgres,mysql" title="PostgreSQL & MySQL" alt="PostgreSQL/MySQL skill-icon">
            </li>
          </ul>
        </div>
      </div>
    </div>

  </div>
</template>

<script setup>
  import AvatarImage from '@/components/global/Pages/Home/AvatarImage.vue';
  import SelfWritingText from '@/components/global/SelfWritingText.vue';

  const words = ['HTML', 'CSS', 'PHP', 'Full Stack'];
</script>
