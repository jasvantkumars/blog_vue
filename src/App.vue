<template>
  <div>
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld />
    <HomeComponent />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import HomeComponent from './components/HomeComponent.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    HomeComponent
  }
}
</script>
