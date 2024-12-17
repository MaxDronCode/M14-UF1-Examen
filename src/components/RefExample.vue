<script setup>
import { ref } from 'vue'

const contador = ref(0)
const incrementar = () => contador.value++
</script>

<template>
  <h2>Ejemplo Ref</h2><br>
  <p>El Contador es: {{ contador }}</p><br>
  <button @click="incrementar">Incrementar</button><br>
</template>

<style scoped></style>
