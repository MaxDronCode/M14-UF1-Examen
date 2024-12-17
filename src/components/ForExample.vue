<script setup>
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
</script>
<template>
<h2>VFor example</h2><br>
<ul>
  <li v-for="product in products" :key="product.id">{{ product.name }} - {{ product.price }}</li>
</ul><br>
</template>
<style scoped>

</style>