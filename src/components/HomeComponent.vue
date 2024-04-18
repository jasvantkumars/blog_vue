<template>
  <h1>Get Checkbox & Radio Button Value</h1>

  <h3>Technology</h3>
  <label for="java">Java</label>

  <input type="checkbox" value="java" v-model="technology" id="java">

  <label for="php">Php</label>
  <input type="checkbox" value="php" v-model="technology" id="php">

  <label for="node">Node</label>
  <input type="checkbox" value="node" v-model="technology" id="node">

  <br /><br />
  <h3>Who I am</h3>

  <label for="student">Student</label>
  <input type="radio" value="student"  v-model="who" name="who" id="student">

  <label for="developer">Developer</label>
  <input type="radio" value="developer"  v-model="who" name="who" id="developer">
  I

  <br /><br />
  <h4>Selected Technology: {{ technology }}</h4>
  <h4>I am a: {{ who }}</h4>

</template>
  
  
  <script>
  export default {
    data() {
      return {
        technology: [],
        who: null
      }
    }
  }
  </script>
  