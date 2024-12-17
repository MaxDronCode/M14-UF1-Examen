<script setup>
// Definimos las props que recibimos
defineProps({
  mensaje: String
})
</script>

<template>
  <div>
    <h2>Componente Hijo</h2>
    <!-- Mostramos la prop recibida -->
    <p>Mensaje recibido: {{ mensaje }}</p>
  </div>
</template>

<style scoped></style>
