<script setup>
defineProps({
  label: { type: String, default: 'Click me' },
  color: { type: String, default: 'indigo' },
})

const colors = {
  indigo: 'bg-indigo-600 hover:bg-indigo-700',
  green: 'bg-green-600 hover:bg-green-700',
  red: 'bg-red-600 hover:bg-red-700',
}
</script>

<template>
  <button class="text-white px-5 py-2 rounded-lg" :class="colors[color] || colors.indigo">
    {{ label }}
  </button>
</template>
