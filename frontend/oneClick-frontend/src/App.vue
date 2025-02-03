<script setup lang="ts">
import HelloWorld from "./components/HelloWorld.vue";
import { ref } from "vue";

const value = ref(0);
</script>

<template>
  <main class="flex items-center justify-center h-screen bg-gray-100">
    <div class="flex flex-col items-center gap-4">
      <p>Value: {{ value }}</p>
      <div class="flex space-x-4">
        <button class="hover:bg-gray-200 border rounded-md p-1"  @click="value++">Increment</button>
        <button class="hover:bg-gray-200 border rounded-md p-1"  @click="value--">Decrement</button>
      </div>
    </div>
  </main>
</template>

<style scoped></style>
