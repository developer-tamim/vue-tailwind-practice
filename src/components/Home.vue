<template>
    <div>
        <!-- <Navbar /> -->
    <HeroSection />
    </div>
</template>

<script>
import Navbar from './Navbar.vue';
import HeroSection from './HeroSection.vue';

export default {
  name: 'App',
  components: {
    Navbar,
    HeroSection,
  },
};
</script>
