<template>
  <div>
    <h2>{{ name }}</h2>
    <h2>{{ user.name }}</h2>
    <button @click="getData()">Call Function</button>
  </div>
</template>

<script>
export default {
  name: 'ChildComponent',
  props: {
    name: String,
    user: Object,
    getData: Function
  }
};
</script>
