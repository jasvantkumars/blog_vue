<template>
    <div class="user-card">
      <h2>{{ data.name }}</h2>
      <h2>{{ data.email }}</h2>
      <button @click="alertName(data.name)">Alert name</button>
    </div>
  </template>
  
  <script>
  export default {
    name: 'UserComponent',
    props: {
      data: Object,
      alertName: Function
    }
  };
  </script>
  
  <style scoped>
  .user-card {
    background-color: #f2f2f2;
    border: 1px solid #ddd;
    padding: 15px;
    margin: 15px;
    border-radius: 5px;
  }
  </style>
  