<!-------------------------------
--- Vue 2 Options API -----
-------------------------------->
<!-- <script>
export default {
  data() {
    const message = "Welcome vue js project";
    return {
      message,
    };
  },
  methods: {
    getData() {
      return "Hello";
    },
  },
};
</script> -->

<!-------------------------------
--- Vue 2 Composition API -----
-------------------------------->
<!-- <script>
export default {
  setup() {
    const message = "Welcome vue js project";
    function getData() {
      return "Hello";
    }
    return {
      message,
      getData,
    };
  },
};
</script> -->

<!-------------------------------
--- Vue 3 Composition API -----
-------------------------------->
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
