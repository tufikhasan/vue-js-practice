<script setup>
const name = "Towfik hasan";
const rawHtml = "<h1>I am a <em>laravel</em> developer</h1>";
</script>

<template>
  <!-- text interpolation -->
  <h3>{{ name }}</h3>
  <div>{{ rawHtml }}</div>
  <!-- output real HTML -->
  <div v-html="rawHtml"></div>
</template>

<style scoped>
h3 {
  color: coral;
}
</style>
