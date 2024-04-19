<template>
  <h1>{{ text }}</h1>
  <div v-html="tag"></div>
  <div v-html="tag2"></div>
</template>

<script>

export default {
  name: "HomeComponent",
  data() {
    return {
     text:"Mukesh kumar",
     tag:"<h1>Mukesh kumar</h1>",
     tag2:"<h1>mukesh@kumar.com</h1>"
    }
  }
}
</script>
