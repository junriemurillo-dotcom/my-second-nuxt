<template>
  <div class="space-y-6">
    <h1 class="text-3xl font-bold">Student Information Website</h1>

    <InfoCard
      title="About This Website"
      description="This website shows how reusable components and props work in Nuxt."
    />
    <InfoCard
      title="Reusable Components"
      description="The same header, footer, and cards are used on every page."
    />
    <InfoCard
      title="Props"
      description="Props pass data like names and colors into a component."
    />

    <div class="flex flex-wrap gap-3">
      <NuxtLink to="/students">
        <AppButton label="View Students" color="indigo" />
      </NuxtLink>
      <AppButton label="Enroll" color="green" />
      <AppButton label="Cancel" color="red" />
    </div>
  </div>
</template>
