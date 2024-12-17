<script setup>
// Definimos el evento que vamos a emitir
import { defineEmits } from 'vue'

const emit = defineEmits(['evento-hijo'])

// Función que emite el evento al padre
const enviarEvento = () => {
  emit('evento-hijo', 'Hola desde el hijo')
}
</script>

<template>
  <div>
    <h2>Componente Hijo</h2>
    <button @click="enviarEvento">Emitir Evento</button>
  </div>
</template>

<style scoped>
button {
  padding: 8px 12px;
  background-color: lightcoral;
  border: none;
  cursor: pointer;
}
</style>
