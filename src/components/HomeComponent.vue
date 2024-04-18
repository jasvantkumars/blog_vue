<template>
  <h1>For Loop in Vue js</h1>

  <ul>
    <li v-for="item in technology" :key="item">
      {{ item }}
    </li>
  </ul>
  <br />

  <br />
  <ul>
    <li v-for="item in user" :key="item.email">
      Name is : {{ item.name }} and Email is : {{ item.email }}
    </li>
  </ul>
</template>

<script>
export default {
  data() {
    return {
      technology: ["java", "php", "node"],
      user: [
        { name: "John", email: "john@example.com" },
        { name: "Jane", email: "jane@example.com" },
      ],
    };
  },
};
</script>