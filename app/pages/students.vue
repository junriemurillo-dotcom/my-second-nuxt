<script setup>
const students = [
  { name: 'Grace Dailo', course: 'BS Information Technology', year: '3rd Year', email: 'gracedailo@gmail.com' },
  { name: 'Jhon Paul Duro', course: 'BS Information Technology', year: '3rd Year', email: 'jhonpaulduro@gmail.com' },
  { name: 'Junrie D. Murillo', course: 'BS Information Technology', year: '3rd Year', email: 'junriemurillo@gmail.com' },
  { name: 'Chonadel Terrado', course: 'BS Information Technology', year: '3rd Year', email: 'chonaterrad@gmail.com' },
]
</script>

<template>
  <div class="space-y-6">
    <h1 class="text-3xl font-bold">Students</h1>

    <div class="grid grid-cols-1 sm:grid-cols-2 gap-6">
      <StudentCard
        v-for="s in students"
        :key="s.email"
        :name="s.name"
        :course="s.course"
        :year="s.year"
        :email="s.email"
      />
    </div>

    <NuxtLink to="/"><AppButton label="Back to Home" color="indigo" /></NuxtLink>
  </div>
</template>
