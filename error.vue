<template>
  <div class="flex flex-col items-center justify-center min-h-screen bg-gray-100 text-gray-800">
    <h1 class="text-6xl font-bold">{{ error.statusCode }}</h1>
    <p class="text-xl mt-4">
      <span v-if="error.statusCode === 404">Page not found</span>
      <span v-else>An error occurred</span>
    </p>
    <button class="btn my-7" @click="handleClearError">Go back to Home</button>
  </div>
</template>

<script setup>
defineProps(["error"]);

const handleClearError = () => clearError({ redirect: "/" });
</script>
