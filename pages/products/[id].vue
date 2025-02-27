<script setup lang="ts">

  const { id } = useRoute().params
  const uri = 'https://fakestoreapi.com/products/' + id

  definePageMeta({
    layout: 'products',
  })

  const { data: product } = await useFetch(uri)

  if(!product.value) {
    throw createError({statusCode: 404, message: 'Product not found!', fatal: true})
  }
</script>

<template>
  <div>
    <ProductDetails :product="product" />
  </div>
</template>
