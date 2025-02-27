<script setup lang="ts">

defineProps(['error'])

const handleClearErrors = () => {
  clearError({redirect: '/'})
}
</script>

<template>
  <div class="max-w-sm mx-auto text-center mt-4 p-6 rounded-md bg-white shadow-md h-full flex flex-col">
    <p class="mt-7 text-4xl font-bold">
      {{ error.statusCode }}
    </p>
    <p class="mt-7 text-6xl">
      Ooops.
    </p>
    <p class="mt-7">
      {{ error.message }}
    </p>
    <button class="px-3 py-2 my-4 text-sm text-white rounded-md bg-[#12b488] shadow-md"  @click="handleClearErrors"> Go Home... </button>
  </div>
</template>
