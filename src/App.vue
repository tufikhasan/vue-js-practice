<script setup>
const result = true;
const day = "sunday";
</script>
<template>
  <h1 v-show="result">Result</h1>
  <h1 v-show="result == 1">Result</h1>

  <h2 v-show="day == 'sunday'">Sunday</h2>
  <h2 v-show="day == 'monday'">Monday</h2>
  <h2 v-show="day == 'tuesday'">Tuesday</h2>
</template>

<style scoped></style>
