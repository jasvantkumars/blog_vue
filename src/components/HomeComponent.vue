<!-- HomeComponent.vue -->
<template>
  <h1>Props And Vue js</h1>
  <StudentComponent :name="name"/>
  <TeacherComponent :name="name" />
</template>

<script>
import StudentComponent from './StudentComponent.vue'
import TeacherComponent from './TeacherComponent.vue'
export default {
  name: "HomeComponent",
  data(){
    return{
      name: "Jasvant Kumar"
    }
  },
  components:{
    StudentComponent,
    TeacherComponent
  }
};
</script>

<style scoped>
h1 {
  color: orange;
}
</style>
