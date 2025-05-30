<template>
  <main>
    <h1 class="font-bold text-2xl border-r-2 pr-2 blink">Bem-vindo ao meu Portfolio!</h1>

    <div class="p-8">

      <Projetos />
      <Habilidades />
      
    </div>
  </main>
</template>

<script setup>
import Habilidades from '../components/HabilidadesComponent.vue'
import Projetos from '../components/ProjetosComponent.vue'
</script>


<!-- animação de escrita -->
<style scoped>
@keyframes blink {
  50% {
    border-color: transparent;
  }
}

.blink {
  animation: blink 0.5s infinite step-end alternate
}
</style>
