<template>
  <h1>CSS Binding</h1>
  <h2 :class="applyStyle">Dynamic Class Binding</h2>
  <button @click="colorfull = !colorfull">Apply Style</button>
</template>

<script>
export default {
  name: "HomeComponent",
  data() {
    return {
      colorfull: true
    };
  },
  computed: {
    applyStyle() {
      return {
        green: this.colorfull,
        err: true,
        other: true
      };
    }
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
.other {
  font-size: 50px;
}

.err {
  color: red;
}
</style>
