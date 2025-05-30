<script setup>
import data from '../assets/data.json'

const habilidades = data.habilidades
</script>

<template>
  <section class="py-8">
    <h2 class="text-2xl font-bold mb-10">Minhas Habilidades</h2>

    <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
      <div v-for="(hab, index) in habilidades" :key="index" class="bg-stone-700 rounded-xl shadow p-5">
        <h3 class="font-semibold mb-2">{{ hab.nome }}</h3>
        <div class="w-full h-2 bg-gray-300 rounded-full">
          <div class="h-2 rounded-full" :class="hab.cor" :style="{ width: hab.nivel + '%' }"></div>
        </div>
        <p class="text-sm text-neutral-400 mt-2">{{ hab.nivel }}%</p>
      </div>
    </div>
  </section>
</template>
