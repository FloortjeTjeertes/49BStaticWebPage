<script setup>
import { RouterLink, RouterView } from 'vue-router'
import MainHeader from '@/components/Header.vue'
import Footer from './components/Footer.vue'
</script>

<template>
  <!-- <div class="flex flex-col min-h-screen"> -->
  <div class="h-screen min-h-fit">
    <MainHeader class="fixed w-full" />
    <main class="flex-1 pt-10 min-h-full dark:bg-gray-950">
      <RouterView />
    </main>
    <Footer />
  </div>
</template>

<style scoped></style>
