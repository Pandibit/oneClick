<script setup lang="ts">
import { Search } from "lucide-vue-next";
import { ShoppingCart } from "lucide-vue-next";
</script>
<template>
  <nav
    class="h-5rem w-[calc(100%-2rem)] fixed font-inter text-black md:px-8 py-2 my-2 rounded-full flex justify-between items-center"
  >
    <router-link class="text-white" to="/">Logo</router-link>
    <div
      class="flex-1 flex items-center justify-center sm:items-stretch sm:justify-center"
    >
      <div class="hidden sm:block sm:ml-6">
        <div class="relative">
          <div
            class="absolute w-full  bg-conic-180 from-mantle via-zinc-50 to-mantle -inset-0.5 rounded-full blur-xs border opacity-80"
          ></div>
          <div
            class="flex gap-6 relative  nav-center md:space-x-10 text-xs text-white items-center bg-black rounded-full pr-3"
          >
            <div
              class="rounded-full pr-4 min-w-[12rem] text-lavaBlack bg-white p-1 m-1 flex items-center justify-between"
            >
              <span>Categories</span>
              <span>+</span>
            </div>
            <router-link to="#">Home</router-link>
            <router-link to="#">About</router-link>
            <router-link to="#">Contact</router-link>
            <router-link to="#">Blog</router-link>
          </div>
        </div>
      </div>
    </div>
    <div class="flex items-center gap-4">
      <span
        class="w-8 h-8 flex items-center justify-center rounded-full bg-gray-100"
      >
        <Search :size="14" :stroke-width="1" />
      </span>
      <span
        class="rounded-full bg-lavaBlack text-white w-8 h-8 flex items-center justify-center p-2"
      >
        <ShoppingCart fill="white" :size="14" :stroke-width="1" />
      </span>
    </div>
  </nav>
</template>
<style scoped>
.nav-center {

}
</style>
