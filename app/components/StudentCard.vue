<script setup>
defineProps({
  name: { type: String, required: true },
  course: { type: String, required: true },
  year: { type: String, required: true },
  email: { type: String, required: true },
})
</script>

<template>
  <div class="bg-white rounded-2xl shadow p-6 text-center">
    <div class="w-20 h-20 rounded-full bg-indigo-100 text-indigo-700 text-3xl font-bold flex items-center justify-center mx-auto">
      {{ name.charAt(0) }}
    </div>
    <h3 class="text-lg font-semibold mt-4">{{ name }}</h3>
    <p class="text-indigo-600 text-sm">{{ course }}</p>
    <p class="text-gray-600 text-sm">{{ year }}</p>
    <p class="text-gray-500 text-sm mt-2">{{ email }}</p>
  </div>
</template>
