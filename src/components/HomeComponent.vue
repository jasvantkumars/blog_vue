<template>
  <h1>Simple Form</h1>

  <p>
    {{ form }}
  </p>
  <form>
    <label>Email:</label>
    <input type="text" placeholder="Enter Email" v-model="form.email" />
    <br />
    <br />
    <label>Password: </label>
    <input type="password" placeholder="Enter Password" v-model="form.password" />
    <br />
    <br />
    <button v-on:click="login" type="button">Login</button>
  </form>
</template>

<script>
export default {
  name: 'HomeComponent',
  data() {
    return {
      form: {
        email: "",
        password: "",
      },
    };
  },
  methods: {
    login() {
      // Login functionality here
      console.log("login", this.form);
    },
  },
};
</script>

<style scoped>
h1 {
  color: orange;
}
</style>
