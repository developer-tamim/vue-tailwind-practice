<template>
  <div id="app" class="bg-white ">
    <navbar></navbar>
    <router-view></router-view>
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue';

export default {
  components: { Navbar },
  name: 'App',
  
};
</script>

<style>
/* Add any global styles here */
</style>
