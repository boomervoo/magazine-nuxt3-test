<script setup lang="ts">

</script>

<template>
  <div class="">
    <header class="shadow-md bg-white">
      <nav class="container mx-auto p-5 flex justify-between">
        <NuxtLink class="text-green-500 font-bold text-xl" to="/">Nuxt Dojo Merch</NuxtLink>
      </nav>
    </header>

    <div class="container mx-auto p-5">
      <slot/>
    </div>

    <footer class="container mx-auto p-5">
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
    </footer>
  </div>
</template>

<style scoped>
.router-link-exact-active {
  color: green;
}
</style>