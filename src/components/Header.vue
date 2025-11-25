<script setup>
import { FwbNavbar, FwbNavbarCollapse, FwbNavbarLink, FwbNavbarLogo } from 'flowbite-vue'
</script>
<template>
  <fwb-navbar>
    <template #logo>
      <fwb-navbar-logo alt="Flowbite logo" image-url="./images/49BLogo.png" link="#">
        49B
      </fwb-navbar-logo>
    </template>
    <template #default="{ isShowMenu }">
      <fwb-navbar-collapse :is-show-menu="isShowMenu">
        <fwb-navbar-link is-active link="/">
          <RouterLink to="/">Home</RouterLink>
        </fwb-navbar-link>
        <fwb-navbar-link link="/np"
          ><RouterLink to="/games"> Our Games</RouterLink>
        </fwb-navbar-link>
      </fwb-navbar-collapse>
    </template>
  </fwb-navbar>
</template>
