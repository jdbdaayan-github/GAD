<template>
  <div class="min-h-screen bg-gray-100 flex items-center justify-center p-4">
    <div class="bg-white shadow-lg rounded-lg w-full max-w-sm p-6">
      <h2 class="text-2xl font-bold text-center mb-6">Login</h2>

      <form @submit.prevent="handleLogin" class="space-y-4">
        <!-- Email -->
        <div class="form-control w-full">
          <label class="label">
            <span class="label-text">Email</span>
          </label>
          <input
            type="email"
            placeholder="Enter your email"
            v-model="email"
            class="input input-bordered w-full"
            required
          />
        </div>

        <!-- Password -->
        <div class="form-control w-full">
          <label class="label">
            <span class="label-text">Password</span>
          </label>
          <input
            type="password"
            placeholder="Enter your password"
            v-model="password"
            class="input input-bordered w-full"
            required
          />
        </div>

        <!-- Remember Me -->
        <div class="form-control w-full">
          <label class="label cursor-pointer justify-start">
            <input type="checkbox" class="checkbox mr-2" v-model="remember" />
            <span class="label-text">Remember Me</span>
          </label>
        </div>

        <!-- Submit Button -->
        <div class="form-control w-full mt-4">
          <button type="submit" class="btn btn-primary w-full">Login</button>
        </div>

        <!-- Links -->
        <p class="text-sm text-center mt-2">
          <router-link to="/forgot" class="text-blue-500 hover:underline">Forgot Password?</router-link>
        </p>
      </form>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'
import { useRouter } from 'vue-router'

const email = ref('')
const password = ref('')
const remember = ref(false)

const router = useRouter()

const handleLogin = () => {
  console.log('Email:', email.value)
  console.log('Password:', password.value)
  console.log('Remember:', remember.value)

  // TODO: call API to validate user
  // Simulate login
  if (email.value === 'admin@example.com' && password.value === '123456') {
    alert('Login successful!')
    router.push('/') // navigate to home/dashboard
  } else {
    alert('Invalid credentials!')
  }
}
</script>

<style scoped>
/* Optional: center vertically */
</style>