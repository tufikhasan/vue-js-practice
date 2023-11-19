<script setup>
const day = "fri";
const weather = "s";
</script>
<template>
  <!-- ternary operator -->
  <!-- <h1>{{ day == "sun" ? "Weekend" : "No weekend" }}</h1>
  <br /> -->

  <!--multiple condition -  ternary operator -->
  <!-- <h1>
    {{ day == "sun" ? "Weekend" : "No weekend" }}
    {{ weather == "s" ? "Today is a sunny day." : "Winter" }}
  </h1>
  <br /> -->

  <!--multiple condition -  ternary operator -->
  <h1>
    {{ day == "sun" ? "Weekend" : day == "fri" ? "Zummah" : "work day" }}
  </h1>
  <br />
</template>

<style scoped>
h1 {
  color: red;
}
</style>
