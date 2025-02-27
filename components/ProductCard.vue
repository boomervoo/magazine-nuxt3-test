<script setup>
const { product } = defineProps(['product'])
</script>

<template>
<div class="p-3 rounded-md bg-white shadow-md h-full flex flex-col text-center">
  <img :src="product.image" alt="product" class="thumb" />
  <p class="font-bold text-gray-500 m-4 truncate"> {{ product.title }}</p>
  <NuxtLink :to="`/products/${product.id}`">
    <p class="px-3 py-2 my-4 text-sm text-white rounded-md bg-[#12b488] shadow-md">View Details</p>
  </NuxtLink>
</div>
</template>

<style>
.thumb {
  max-height: 120px;
  max-width: 70%;
  margin: 0 auto;
}

</style>