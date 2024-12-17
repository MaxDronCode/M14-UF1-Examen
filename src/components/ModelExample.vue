<script setup>
import { ref } from 'vue'

const text = ref('')
</script>
<template>
  <h2>VModel Example</h2><br>
  <p>The text is : {{ text }}</p><br>
  <input type="text" v-model="text" placeholder="Type here..."><br>
</template>
<style scoped></style>
