<script setup lang="ts">

</script>

<template>
  <div>
    <header class="shadow-md bg-white">
      <nav class="container mx-auto p-5 flex justify-between ">
        <NuxtLink class="text-green-500 text-xl font-bold" to="/">Nuxt Dojo</NuxtLink>
        <ul class="flex gap-10 items-center">
          <li>
            <NuxtLink to="/">Home</NuxtLink>
          </li>
          <li>
            <NuxtLink to="/about">About</NuxtLink>
          </li>
          <li>
            <NuxtLink to="/programm">Programm</NuxtLink>
          </li>
          <li>
            <NuxtLink to="/products">Products</NuxtLink>
          </li>
        </ul>
      </nav>
    </header>
    <div class="container mx-auto p-5">
      <slot/>
    </div>
  </div>
</template>

<style scoped>
  .router-link-exact-active {
    color: green;
  }
</style>