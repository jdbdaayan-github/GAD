<script setup>
import Navbar from '@/components/partials/public/Navbar.vue'
import Footer from '../partials/public/Footer.vue';
</script>

<template>
  <Navbar />
  <div class="flex">
    <main class="flex-1 p-4 w-lg mx-5">
      <router-view />
    </main>
  </div>
  <Footer />
</template>