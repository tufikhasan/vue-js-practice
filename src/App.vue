<script setup>
const result = true;
const day = "friday";
</script>
<template>
  <h1 v-if="result">Result</h1>
  <h1 v-if="result == 1">Result</h1>

  <h2 v-if="day == 'sunday'">Sunday</h2>
  <h2 v-else-if="day == 'monday'">Monday</h2>
  <h2 v-else-if="day == 'tuesday'">Tuesday</h2>
  <h2 v-else>Today Is a {{ day }}</h2>
</template>

<style scoped></style>
