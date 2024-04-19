<!-- HomeComponent.vue -->
<template>
  <div>
    <h1>Pass Data to child Component</h1>
    <!-- Here's where you use the ChildComponent -->
    <ChildComponent name="anil sidhu" :user="user" :get-data="getData" />
  </div>
</template>

<script>
import ChildComponent from './ChildComponent.vue'

export default {
  name: "HomeComponent",
  components: {
    ChildComponent
  },
  data() {
    return {
      user: {
        name: 'Peter',
        email: 'peter@test.com'
      }
    }
  },
  methods: {
    getData() {
      console.warn("parent function called")
    }
  }
}
</script>
