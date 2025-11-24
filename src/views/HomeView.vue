<script setup>
import HeroSection from '@/components/HeroSection.vue'
import { FwbCard, FwbHeading, FwbP } from 'flowbite-vue'
</script>

<template>
  <hero-section />
  <section>
    <fwb-heading tag="h1">About Us!</fwb-heading>
    <fwb-p>home</fwb-p>
  </section>
  <fwb-card href="#" class="w-sm">
    <div class="p-5">
      <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
        Noteworthy technology acquisitions 2021
      </h5>
      <p class="font-normal text-gray-700 dark:text-gray-400">
        Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse
        chronological order.
      </p>
    </div>
  </fwb-card>
</template>
