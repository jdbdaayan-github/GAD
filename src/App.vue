<script setup>
import { useAuthStore } from '@/stores/auth'
import PublicLayout from '@/components/layouts/PublicLayout.vue'
import AdminLayout from '@/components/layouts/AdminLayout.vue'
import { useRoute } from 'vue-router'

const auth = useAuthStore()
const route = useRoute()
</script>

<template>
  <component :is="route.meta.layout === 'admin' && auth.isLoggedIn ? AdminLayout : PublicLayout" />
</template>