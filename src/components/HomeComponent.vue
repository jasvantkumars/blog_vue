<template>
  <h1>CSS Binding</h1>
  <h2 :class="{ green: colorful }">Dynamic Class Binding</h2>
</template>

<script>
export default {
  name: "HomeComponent",
  data() {
    return {
      colorful: true
    };
  }
};
</script>

<style scoped>
h1 {
  color: orange;
}
.green {
  background-color: green;
  width: 200px;
  padding: 10px;
}
</style>
