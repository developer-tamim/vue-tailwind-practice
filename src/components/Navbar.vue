<template>
  <header class="absolute inset-x-0 top-0 z-50">
    <nav class="flex items-center justify-between p-6 lg:px-8" aria-label="Global">
      <div class="flex lg:flex-1">
        <a href="#" class="-m-1.5 p-1.5">
          <span class="sr-only">Your Company</span>
          <!-- <img class="h-8 w-auto" src="https://tailwindui.com/img/logos/mark.svg?color=indigo&shade=600" alt=""> -->
           <div class="font-bold text-3xl sm:text-2xl">
            <span class="text-green-700">Tawsif</span><span>Tamim</span>
           </div>
        </a>
      </div>
      <div class="flex lg:hidden">
        <button @click="toggleMobileMenu" type="button" class="-m-2.5 inline-flex items-center justify-center rounded-md p-2.5 text-gray-700 ">
          <span class="sr-only">Open main menu</span>
          <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" aria-hidden="true">
            <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5" />
          </svg>
        </button>
      </div>
      <div class="hidden lg:flex lg:gap-x-12">
        <a href="#" class="text-sm font-semibold leading-6 text-gray-900">Home</a>
        <a href="#" class="text-sm font-semibold leading-6 text-gray-900">Services</a>
        <a href="#" class="text-sm font-semibold leading-6 text-gray-900">Resume</a>
        <a href="#" class="text-sm font-semibold leading-6 text-gray-900">Worrk</a>
        <a href="#" class="text-sm font-semibold leading-6 text-gray-900">Contact</a>
      </div>
      
    </nav>
    <MobileMenu :isOpen="isMobileMenuOpen" @close="toggleMobileMenu"/>
  </header>
</template>

<script>
import MobileMenu from './MobileMenu.vue';

export default {
  components: {
    MobileMenu,
  },
  data() {
    return {
      isMobileMenuOpen: false,
    };
  },
  methods: {
    toggleMobileMenu() {
      this.isMobileMenuOpen = !this.isMobileMenuOpen;
    },
  },
};
</script>
