<script setup>
import { ref } from "vue";
const number = ref();
</script>
<template>
  <h1 v-show="number">
    {{ number }} is {{ number < 0 ? "negative" : "" }}
    {{ number % 2 == 0 ? "Even" : "Odd" }} number
  </h1>
  <input
    type="number"
    v-model="number"
    placeholder="Input a number to check Even or Odd"
  />
</template>

<style scoped>
input {
  width: 300px;
  padding: 1rem;
}
</style>
