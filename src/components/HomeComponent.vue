<template>
  <div>
    <h1 v-on:mousemove="getConsole()">Home Component</h1>
    <button v-on:click="getData()">Click Me</button>
    <button v-on:dblclick="getData('Button double clicked')">Double Click Me</button>
    <h2>{{ count }}</h2>
  </div>
</template>

<script>
export default {
  name: "HomeComponent", // Changed from "Home" to "HomeComponent"
  data() {
    return {
      count: 0
    }
  },
  methods: {
    getData(data) {
      this.count++;
      console.log(data);
    },
    getConsole() {
      console.warn("Function called");
    }
  }
}
</script>

<style scoped>
h1 {
  color: orange;
}
</style>
