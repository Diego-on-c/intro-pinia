<script lang="ts" setup>

import { useCounterStore } from '../stores/counter';

const counterStore = useCounterStore();

const increaseBy = (value) => {
  counterStore.increment(value);
}
</script>

<template>
  <h1>
    Couter View: {{ counterStore.count }}!!!
  </h1>

  <button @click="increaseBy(1)">+1</button> <span></span>
  <button @click="increaseBy(2)">+2</button> <span></span>
  <button @click="increaseBy(5)">+5</button>
</template>


<style scoped>
button{
  font-size: 30px;
}
</style>