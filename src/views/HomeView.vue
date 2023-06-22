<script lang="ts" setup>

import { useCounterStore } from '../stores/counter';

const counterStore = useCounterStore();


</script>

<template>
  <div>
    <h1> Home View: {{ counterStore.count }} </h1>
    <h3> Double Count: {{ counterStore.doubleCount }}</h3>
  </div>
</template>

<style scoped>
div{
  text-align: center;
  width: 100%;
  font-size: 32px;
}
</style>


