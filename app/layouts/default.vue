<template>
  <div class="min-h-screen bg-gray-100 text-gray-800 flex flex-col">
    <AppHeader />
    <main class="max-w-4xl w-full mx-auto p-6 flex-1">
      <slot />
    </main>
    <AppFooter />
  </div>
</template>
