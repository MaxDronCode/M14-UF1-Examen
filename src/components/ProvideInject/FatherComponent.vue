<!-- App.vue -->
<script setup>
import { ref, provide } from 'vue'
import ChildComponent from './ChildComponent.vue'

// Creamos una referencia reactiva
const mensaje = ref('Hola desde el componente padre')

// Usamos `provide` para compartir la variable con los hijos
provide('mensajeCompartido', mensaje)

// Función para cambiar el mensaje
const cambiarMensaje = () => {
  mensaje.value = 'Mensaje actualizado desde el padre'
}
</script>

<template>
  <div>
    <h1>Componente Padre</h1>
    <p>Mensaje en el Padre: {{ mensaje }}</p>
    <button @click="cambiarMensaje">Actualizar Mensaje</button>
    <ChildComponent />
  </div>
</template>

<style scoped></style>
