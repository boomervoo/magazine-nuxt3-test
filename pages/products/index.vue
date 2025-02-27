<script setup>
definePageMeta({
  layout: 'products',
})

const { data: products } = await useFetch('https://fakestoreapi.com/products')

</script>

<template>
  <div>
    <div class="grid grid-cols-5 gap-5">
      <div v-for="product in products">
        <ProductCard :product="product" />
      </div>
    </div>
  </div>
</template>

<style scoped>

</style>