<template>
  <h1 v-if="show">If Condtion</h1>

  <h1 v-else>else Condtion</h1>

  <button v-on:click="show = !show">Toogle</button>
</template>

<script>
export default {
  name: "HomeComponent",
  data() {

    return {
      show: true

    }

  }
}
</script>

<style scoped>
h1 {
  color: orange;
}
</style>