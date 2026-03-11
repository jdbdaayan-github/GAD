<script setup>
import Navbar from '@/components/partials/admin/Navbar.vue'
</script>

<template>
  <Navbar />
  <div class="flex">
    <main class="flex-1 p-4">
      <router-view />
    </main>
  </div>
</template>