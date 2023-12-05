<script setup></script>

<template>
  <h2>When working event always use v-show condition not v-if</h2>
  <h2>v-if can use template tag but v-show not working template tag</h2>
  <template v-if="true">
    <h1>v-if: working template tag</h1>
  </template>
  <div v-if="true">
    <h1>v-if: show all tag with parent tag</h1>
  </div>

  <br />

  <template v-show="true">
    <h1>v-show: not working template tag</h1>
  </template>
  <div v-show="true">
    <h1>v-show: always show all tag with parent tag</h1>
  </div>
</template>

<style scoped>
h2 {
  color: red;
}
</style>
