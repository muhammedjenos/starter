<template>
  <div v-if="isDevelopment" class="fixed z-50 flex items-center justify-center p-3 font-mono text-lg text-white bg-gray-800 rounded-full bottom-1 left-1 dark:text-light size-10">
    <div class="block sm:hidden">xs</div>
    <div class="hidden sm:block md:hidden">sm</div>
    <div class="hidden md:block lg:hidden">md</div>
    <div class="hidden lg:block xl:hidden">lg</div>
    <div class="hidden xl:block 2xl:hidden">xl</div>
    <div class="hidden 2xl:block">2xl</div>
  </div>
</template>

<script setup>
const isDevelopment = process.env.NODE_ENV !== 'production'
</script>