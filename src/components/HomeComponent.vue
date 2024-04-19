<template>
  <h1>{{ childUser }}</h1>
  <UserComponent :getUser="getUserName" />
</template>

<script>
import UserComponent from './UserComponent.vue'
export default {
  name: "HomeComponent",
  data() {
    return {
      childUser: ""
    }
  },
  components: {
    UserComponent
  },
  methods: {
    getUserName(name) {
      this.childUser = name
    }
  }
};
</script>

<style scoped>
h1 {
  color: orange;
}
</style>
