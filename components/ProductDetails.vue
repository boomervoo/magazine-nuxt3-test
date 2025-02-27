<script setup lang="ts">
const { product } = defineProps(["product"]);
</script>

<template>
  <div class="p-3 rounded-md bg-white shadow-md h-full flex flex-col">
    <div class="grid grid-cols-2 gap-10">
      <div clas="p-7">
        <img :src="product.image" alt="img" class="mx-auto my-7">
      </div>
      <div clasd="p-7">
        <h2 class="text-4xl my-7"> {{ product.title }}</h2>
        <p class="text-xl my-7"> Price - ${{ product.price }}</p>
        <h3 class="font-bold border-b-2 mb-4 pb-4"> Product description:</h3>
        <p class="mb-7"> {{ product.description }}</p>
      </div>

    </div>
  </div>
</template>

<style>
img {
  max-width: ;
}
</style>
