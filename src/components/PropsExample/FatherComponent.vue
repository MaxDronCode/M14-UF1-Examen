<script setup>
import ChildComponent from './ChildComponent.vue'

// Datos que queremos pasar al hijo
const mensajePadre = 'Hola desde el componente padre'
</script>

<template>
  <div>
    <h1>Componente Padre</h1>
    <!-- Pasamos la prop al componente hijo -->
    <ChildComponent :mensaje="mensajePadre" />
  </div>
</template>

<style scoped></style>
