<script setup>
const message = "Welcome vue js project";
function getData() {
  return "Hello";
}
</script>

<template>
  <h1>{{ message }}</h1>
  <h1>{{ getData() }}</h1>
</template>

<style scoped>
h1 {
  color: red;
}
</style>
