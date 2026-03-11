<template>
  <footer class="bg-purple-900 text-white mt-8">
    <div class="max-w-7xl mx-auto px-4 py-8 grid grid-cols-1 md:grid-cols-3 gap-8">
      
      <!-- Column 1: Address -->
      <div>
        <h3 class="text-lg font-bold mb-2">Our Address</h3>
        <p class="text-sm">
          DSWD Central Office,<br>
          IBP Road, Batasan Pambansang Complex,<br>
          Constitution Hills, Quezon City, Philippines, 1126
        </p>
      </div>

      <!-- Column 2: Contact Info -->
      <div>
        <h3 class="text-lg font-bold mb-2">Contact Us</h3>
        <p class="text-sm">
          Tel. Nos.: 8931-9105 to 107 <br>
          Local VoIP: 10130 <br>
          Email: <a href="mailto:records@dswd.gov.ph" class="underline hover:text-yellow-300">records@dswd.gov.ph</a>
        </p>
      </div>

      <!-- Column 3: Google Map -->
      <div>
        <h3 class="text-lg font-bold mb-2">Location Map</h3>
        <div class="w-full h-48 md:h-40 rounded overflow-hidden shadow-inner">
          <iframe
            class="w-full h-full"
            loading="lazy"
            allowfullscreen
            referrerpolicy="no-referrer-when-downgrade"
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3861.786553541282!2d121.06892611534347!3d14.651951189807244!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3397b6833f619d8b%3A0x4691848c7e9c1740!2sDSWD%20Central%20Office!5e0!3m2!1sen!2sph!4v1700000000000!5m2!1sen!2sph"
          ></iframe>
        </div>
      </div>

    </div>

    <div class="text-center text-sm bg-purple-800 py-2 mt-4">
      &copy; {{ new Date().getFullYear() }} DSWD GAD Information Hub. All rights reserved.
    </div>
  </footer>
</template>

<script setup lang="ts">
// nothing required here
</script>

<style scoped>
/* optional: smooth iframe border */
iframe {
  border: 0;
}
</style>