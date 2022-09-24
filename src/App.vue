<template>
  <div class="relative bg-gray-100 py-24 font-sans w-full">
    <banner></banner>
    <about-me></about-me>
    <my-skills></my-skills>
    <recent-work></recent-work>
  </div>
</template>

<script>
import banner from './components/Banner.vue'
import aboutMe from './components/AboutMe.vue'
import mySkills from './components/MySkills.vue'
import recentWork from './components/RecentWork.vue'

export default {
  name: 'App',
  components: {
    banner,
    aboutMe,
    mySkills,
    recentWork
  }
}
</script>
