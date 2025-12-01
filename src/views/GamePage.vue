<script setup>
import { FwbHeading, FwbP, FwbImg, FwbButton } from 'flowbite-vue'
import Carousel from '@/components/ImageCarousel.vue'
</script>
<template class="flex flex-center items-center">
  <Carousel />
  <section>
    <figure class="relative max-w-sm transition-all duration-300 w-100">
      <fwb-img alt="flowbite-vue" src="https://picsum.photos/300/200" />
      <figcaption class="absolute px-4 text-lg text-white bottom-6">
        <fwb-heading>running beehind🐝</fwb-heading>
      </figcaption>
    </figure>
    <fwb-p>
      Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer est turpis, mollis vel
      euismod nec, convallis a metus. Maecenas ut lectus at sem vulputate volutpat. Aliquam
      convallis neque non neque tincidunt egestas. Sed pretium euismod dui, sagittis mollis diam
      mollis quis. Sed ut laoreet justo. Phasellus et felis a mauris viverra faucibus sit amet ac
      felis. In fringilla, arcu ut malesuada finibus, tortor neque rhoncus nulla, ut tincidunt eros
      leo non enim. Vestibulum commodo mauris eu tempus maximus. Vivamus sit amet est mollis,
      consequat ligula quis, tempor velit. Praesent mattis nulla porttitor enim finibus aliquam.
      Phasellus auctor lacus mi, nec pretium elit pulvinar nec. Morbi rutrum, lacus non accumsan
      mattis, urna metus maximus augue, at feugiat lacus tellus sed justo.
    </fwb-p>
    <router-link to="/runningBeehind">
      <fwb-button color="default">read More!</fwb-button>
    </router-link>
  </section>
</template>
