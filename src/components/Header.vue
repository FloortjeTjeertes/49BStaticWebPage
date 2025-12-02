<script setup>
import {
  FwbNavbar,
  FwbNavbarCollapse,
  FwbNavbarLink,
  FwbNavbarLogo,
  FwbDropdown,
} from 'flowbite-vue'
</script>
<template>
  <fwb-navbar solid>
    <template #logo>
      <fwb-navbar-logo alt="Flowbite logo" image-url="./images/49BLogo.png" link="/">
        49B
      </fwb-navbar-logo>
    </template>
    <template #default="{ isShowMenu }">
      <fwb-navbar-collapse class="hidden md:flex md:space-x-4" :is-show-menu="isShowMenu">
        <fwb-navbar-link is-active link="/">
          <RouterLink to="/">Home</RouterLink>
        </fwb-navbar-link>
        <fwb-navbar-link link="/">
          <RouterLink to="/games">games</RouterLink>
        </fwb-navbar-link>
        <fwb-navbar-link link="/">
          <RouterLink to="/about">about</RouterLink>
        </fwb-navbar-link>
        <fwb-dropdown>
          <template #trigger>
            <fwb-button color="light">
              <fwb-navbar-link link="#"> Our Games </fwb-navbar-link>
            </fwb-button>
          </template>
          <nav class="py-2 text-sm text-gray-700 dark:text-gray-200">
            <router-link
              to="/runningBeehind"
              class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white"
              >running beehind
            </router-link>
          </nav>
        </fwb-dropdown>
      </fwb-navbar-collapse>
    </template>
  </fwb-navbar>
</template>
