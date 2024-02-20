
<script setup>
import { ref } from "vue";

let count = ref(0);
</script>

<template>
  <div class="text-center">
    <h4 class="text-danger">The current count is</h4>
    <h4>{{ count }}</h4>
    <!-- <button class="btn btn-red-500 mx-1 w-25">-</button> -->
    <button
      @click="count--"
      class="bg-transparent hover:bg-red-500 text-white-700 font-semibold hover:text-white py-2 px-4 border border-red-500 hover:border-transparent rounded"
    >
      -
    </button>
    <button
      @click="count++"
      class="bg-transparent hover:bg-blue-500 text-blue-700 font-semibold hover:text-white py-2 px-4 border border-blue-500 hover:border-transparent rounded mx-2"
    >
      +
    </button>

    <!-- <button class="btn btn-success mx-1 w-25" @click="count++">+</button> -->
  </div>
</template>
