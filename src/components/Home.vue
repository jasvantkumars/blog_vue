<template>
    
    <h1>Email {{ email }}</h1>
    <h1>Email {{ mobile }}</h1>
    <h1>Name {{ getName("Jassu") }}</h1>

  </template>
  
  <script>
  export default {
    name: 'HomE',
    data()
    {
        return{
            email:'jas@gmail.com'
            mobile:9555760921
            getName:function(j) {
                return j
            }
        }
    }
   
  }
  </script>

<style scoped>
h1{
  color: orange;
}
</style>