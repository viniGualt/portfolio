<script setup>
import data from '../assets/data.json'

const projetos = data.projetos
</script>

<template>
    <h1 class="text-2xl font-bold mb-6">Meus Projetos</h1>
    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 max-w-6xl mx-auto">
        <div v-for="(projeto, index) in projetos" :key="index"
            class="bg-stone-700 rounded-xl shadow-lg p-6 text-white flex flex-col justify-between">
            <div>
                <h2 class="text-2xl font-semibold mb-2">{{ projeto.nome }}</h2>
                <p class="text-sm text-neutral-400 mb-4">Linguagens: {{ projeto.linguagens.join(', ') }}</p>
            </div>
            <a :href="projeto.github" target="_blank"
                class="mt-4 inline-block bg-fuchsia-800 text-white text-center py-2 px-4 rounded hover:bg-fuchsia-900 transition">
                Ver no GitHub
            </a>
        </div>
    </div>
</template>