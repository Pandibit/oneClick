<script setup lang="ts">
import Navbar from "./components/Navbar/Navbar.vue";
</script>

<template>
  <div class="px-4 font-inter bg-black">
    <Navbar />

    <router-view />
  </div>
</template>

<style scoped></style>
