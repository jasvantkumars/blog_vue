<template>
  <h1>Two Way Binding</h1>

  <input type="text" v-model="count" />
  <h2>{{ count }}</h2>

</template>

<script>
export default {

  name: "HomeComponent",
  data() {
    return {

      count: 10

    }
  }
}

</script>

<style scoped>
body {
  font-family: sans-serif;
}
</style>