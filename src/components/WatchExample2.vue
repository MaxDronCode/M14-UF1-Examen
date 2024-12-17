<script setup>
import { ref, watch } from 'vue'

// Creamos una variable reactiva
const contador = ref(0)

// Observamos los cambios en la variable 'contador'
watch(contador, (nuevoValor, valorAnterior) => {
  console.log(`El contador cambió de ${valorAnterior} a ${nuevoValor}`)
})

// Función para incrementar el contador
const incrementar = () => {
  contador.value++
}
</script>

<template>
  <div>
    <h1>Ejemplo de watch</h1>
    <p>Contador: {{ contador }}</p>
    <button @click="incrementar">Incrementar</button>
  </div>
</template>

<style scoped>
button {
  padding: 8px 12px;
  background-color: lightblue;
  border: none;
  cursor: pointer;
}
</style>
