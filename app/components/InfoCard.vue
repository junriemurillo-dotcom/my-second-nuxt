<script setup>
defineProps({
  title: { type: String, required: true },
  description: { type: String, required: true },
})
</script>

<template>
  <div class="bg-white rounded-2xl shadow p-6">
    <h2 class="text-xl font-semibold text-indigo-600">{{ title }}</h2>
    <p class="text-gray-600 mt-2">{{ description }}</p>
  </div>
</template>
