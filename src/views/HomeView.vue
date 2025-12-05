<script setup>
import HeroSection from '@/components/HeroSection.vue'
import { FwbCard, FwbHeading, FwbP, FwbImg, FwbButton } from 'flowbite-vue'
</script>

<template>
  <hero-section />

  <!-- about -->
  <section class="p-5 flex flex-col flex-center md:flex-row-reverse min-h-100 pb-20 pt-20">
    <fwb-img alt="flowbite-vue" src="https://picsum.photos/300/200" class="max-h-40" />

    <section class="md:w-1/2">
      <fwb-heading tag="h2">About Us!</fwb-heading>
      <fwb-p class="md:w-1/2">
        49B is a game studio based in Rotterdam which consists of 11 people. We combined our skillsets as designers, artists and
        developers with the help of our producer to make "Running Beehind", a 3D platformer game with a speed-based delivery objective.
      </fwb-p>
    </section>
  </section>

  <!-- cards -->
  <section class="flex flex-col w-full md:max-w-full pb-10 justify-center items-center">
    <!-- <fwb-heading tag="h2" class="pb-10 md:max-w-full pl-200">Our Projects!</fwb-heading> -->
    <fwb-heading tag="h2" class="pb-10 md:min-w-100">Our Projects!</fwb-heading>

    <section
      class="flex flex-col md:flex-row items-center md:min-h-contain md:min-w-full md:justify-evenly gap-10 items-stretch"
    >
      <fwb-card
        img-alt="banner"
        img-src="./images/bannerRunningBeehind.png"
        variant="image"
        href="#"
        class="basis-1/2 max-w-24 min-h-full"
      >
        <div class="p-5">
          <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
            Running Beehind
          </h5>
          <p class="font-normal text-gray-700 dark:text-gray-400 pb-10">
            An exciting platforming game set in an world where fantasy and technology combine!
          </p>
          <router-link to="/games"
            ><fwb-button color="default">public tests available!</fwb-button></router-link>
        </div>
      </fwb-card>
      <!-- Not needed yet
      <fwb-card
        href="#"
        img-alt="placeholder"
        img-src="https://placehold.co/600x400"
        variant="image"
        class="basis-1/2 max-w-24 min-h-full"
      >
      
        <div class="p-5">
          <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
            More Coming Soon!
          </h5>
          <p class="font-normal text-gray-700 dark:text-gray-400 pb-10">
            More games coming soon! check out the game pages for all our current games!
          </p>
          <router-link to="/games"
            ><fwb-button color="default">public tests available!</fwb-button></router-link
          >
        </div>
      </fwb-card>
       -->
    </section>
  </section>
</template>
