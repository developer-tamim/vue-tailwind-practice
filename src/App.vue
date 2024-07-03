<template>
  <div id="app" class="bg-white ">
    <Navbar />
    <HeroSection />
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue';
import HeroSection from './components/HeroSection.vue';

export default {
  name: 'App',
  components: {
    Navbar,
    HeroSection,
  },
};
</script>

<style>
/* Add any global styles here */
</style>
