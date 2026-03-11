<script setup lang="ts">
import BpLogo from '@/components/icons/bpLogo.vue';
import dswdLogo from '@/components/icons/dswdLogo.vue';
</script>

<template>
  <div class="sticky top-0 z-50 bg-purple-900 shadow-md">
    <div class="navbar px-4 md:px-8">
      <!-- Left side: Logos + Title -->
      <div class="flex-1 flex items-center gap-2">
        <dswdLogo class="w-10 h-10" />
        <BpLogo class="w-10 h-10" />
        <div class="flex flex-col">
          <b class="text-white text-lg md:text-xl">
            Administrative Service
          </b>
          <span class="text-yellow-300 text-sm md:text-base">
            Gender and Development Information Hub
          </span>
        </div>
      </div>

      <!-- Right side: Menu for medium+ screens -->
      <div class="hidden md:flex flex-none">
        <ul class="menu menu-horizontal px-1 gap-2">
          <li><router-link to="/" class="text-white hover:text-yellow-300">Home</router-link></li>
          <li><router-link to="/about" class="text-white hover:text-yellow-300">About</router-link></li>
          <li><router-link to="/resources" class="text-white hover:text-yellow-300">Resources</router-link></li>
        </ul>
      </div>

      <!-- Mobile menu button -->
      <div class="md:hidden flex-none">
        <div class="dropdown dropdown-end">
          <label tabindex="0" class="btn btn-ghost btn-square">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-white" fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"/>
            </svg>
          </label>
          <ul tabindex="0" class="dropdown-content menu p-2 shadow bg-purple-900 rounded-box w-52 mt-2">
            <li><router-link to="/" class="text-white hover:text-yellow-300">Home</router-link></li>
            <li><router-link to="/about" class="text-white hover:text-yellow-300">About</router-link></li>
            <li><router-link to="/resources" class="text-white hover:text-yellow-300">Resources</router-link></li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
/* Optional: smooth dropdown shadow */
</style>