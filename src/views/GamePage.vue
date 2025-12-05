<script setup>
import { FwbHeading, FwbP, FwbImg, FwbButton } from 'flowbite-vue'
import Carousel from '@/components/ImageCarousel.vue'
</script>
<template class="flex flex-center items-center">
  <Carousel />
  <section>
    <figure class="relative max-w-sm transition-all duration-300 w-100">
      <fwb-img alt="flowbite-vue" src="./images/bannerRunningBeehind.png" />
      <figcaption class="absolute px-4 text-lg text-white top-4">
        <fwb-heading>Running Beehind</fwb-heading>
      </figcaption>
    </figure>
    <div id="desc">
      <fwb-p>
      Running behind is a 3D platformer game with a speed-based delivery objective. Accept orders, retrieve and deliver them
      in a timely manner to get good reviews, and therefore, a higher star rating. 
      </fwb-p>
      <router-link to="/runningBeehind">
        <fwb-button color="default">read More!</fwb-button>
      </router-link>
    </div>
  </section>
</template>
