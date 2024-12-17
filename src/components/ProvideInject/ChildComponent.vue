<!-- ChildComponent.vue -->
<script setup>
import { inject } from 'vue'

// Usamos `inject` para obtener el valor compartido
const mensajeHeredado = inject('mensajeCompartido')
</script>

<template>
  <div>
    <h2>Componente Hijo</h2>
    <p>Mensaje desde el Padre: {{ mensajeHeredado }}</p>
  </div>
</template>

<style scoped></style>
