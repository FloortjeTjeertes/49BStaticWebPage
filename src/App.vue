<script setup>
import { RouterLink, RouterView } from 'vue-router'
import MainHeader from './views/Header.vue'
</script>

<template>
  <div class="flex flex-col min-h-screen">
    <MainHeader />
    <main class="flex-1 pt-30">
      <RouterView />
    </main>
  </div>
</template>

<style scoped></style>
