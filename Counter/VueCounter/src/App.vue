<script setup>
import { ref } from 'vue'
const count = ref(0);

const subToCount = () => {
  count.value = count.value - 1;
};

const addToCount = () => {
  count.value = count.value + 1;
};

</script>

<template>
  <main>
    <h4>
      Count is ...
    </h4>
    <h1>{{ count }}</h1>
    <button @click="count--">-</button>
    <button @click="count++">+</button>
  </main>
</template>

<style scoped>
  main{
    background-color: aqua;
  }
</style>