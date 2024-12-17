<script setup>
import ChildComponent from './ChildComponent.vue'

// Función para manejar el evento emitido por el hijo
const recibirEvento = (dato) => {
  console.log('Evento recibido del hijo:', dato)
}
</script>

<template>
  <div>
    <h1>Componente Padre</h1>
    <!-- Escuchamos el evento 'evento-hijo' -->
    <ChildComponent @evento-hijo="recibirEvento" />
  </div>
</template>

<style scoped></style>
