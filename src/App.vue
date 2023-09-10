<script setup>
import { ref } from 'vue';

 const count = ref(0);

</script>

<template>
  <div class="w-fit mx-auto items-center flex flex-col mt-32">
    <h1 className="text-red-400 mt-4 text-2xl font-semibold"> The current count is </h1>
    <p class="font-bold text-3xl "> {{ count }} </p>
    <div class="space-x-3 mt-4">
      <button @click="count--" class="w-fit px-4 py-1 bg-red-500 rounded text-white font-bold"> - </button>
      <button @click="count++" class="w-fit px-4 py-1 bg-green-500 rounded text-white font-bold"> + </button>
    </div>
  </div>
</template>