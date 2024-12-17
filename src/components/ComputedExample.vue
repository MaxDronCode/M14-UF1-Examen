<script setup>
import { ref, computed } from 'vue'
const products = [
  {
    id: 1,
    name: 'Laptop',
    price: 399
  },
  {
    id: 2,
    name: 'Phone',
    price: 1399
  },
  {
    id: 3,
    name: 'Tablet',
    price: 799
  }
]

const filterPrice = ref(0)

const filteredProducts = computed(() => {
  return products.filter(product => product.price > filterPrice.value)
})
</script>
<template>
<h2>Computed Filter Example</h2><br>
<input type="text" v-model="filterPrice"><br>
<ul>
  <li v-for="product in filteredProducts" :key="product.id">{{ product.name }} - {{ product.price }}</li>
</ul><br>
</template>
<style scoped>

</style>