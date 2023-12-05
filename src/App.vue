<script setup>
const data = {
  name: "Towfik",
  age: 25,
};
</script>

<template>
  <h1
    :class="[
      data.name === 'Towfik' ? 'btn-primary' : 'btn-secondary',
      data.age === 25 ? 'adult' : 'child',
    ]"
  >
    Hello
  </h1>
</template>

<style scoped></style>
