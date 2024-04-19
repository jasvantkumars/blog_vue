<template>
  <h2>User Component</h2>
  <button v-on:click="getUser(userName)">Send User Name</button>
</template>

<script>
export default {
  name: 'UserComponent',
  data() {
    return {
      userName: "Jasvant Kumar"
    }
  },
  props: {
    getUser: Function
  }
};
</script>
