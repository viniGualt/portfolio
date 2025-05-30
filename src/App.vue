<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Navbar from './components/NavbarComponent.vue'
</script>

<template>
  <main class="flex h-screen bg-stone-800 text-white">
    <Navbar />

    <div class="flex-1 p-6">
      <RouterView />
    </div>

  </main>
</template>