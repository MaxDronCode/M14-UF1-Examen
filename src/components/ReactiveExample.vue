<script setup>
import { reactive } from 'vue'

const person = reactive({
  name: 'Max',
  age: 31
})

const addAge = () => person.age++
</script>

<template>
<h2>Ejemplo Reactive</h2><br>
<p>Name is {{ person.name }}</p><br>
<p>Age is {{ person.age }}</p><br>
<button @click="addAge">Add age</button><br>
</template>

<style scoped>

</style>