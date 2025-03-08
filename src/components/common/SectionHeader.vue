<script setup lang="ts">
defineProps({
  title: {
    type: String,
    required: true
  },
  subtitle: {
    type: String,
    default: ''
  }
})
</script>

<template>
  <div class="text-center mb-12">
    <h2 class="text-3xl font-bold text-primary">{{ title }}</h2>
    <div class="w-20 h-1 bg-accent mx-auto mt-3 mb-6"></div>
    <p v-if="subtitle" class="text-gray-600 max-w-3xl mx-auto">{{ subtitle }}</p>
  </div>
</template>
