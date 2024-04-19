<template>
  <div>
    <h1>Pass Data to Child Component</h1>
    <ul>
      <li v-for="item in users" :key="item.name">
        <!-- Pass the method as a prop -->
        <UserComponent :data="item" :alertName="getData" />
      </li>
    </ul>
  </div>
</template>

<script>
import UserComponent from './UserComponent.vue'

export default {
  name: "HomeComponent",
  components: {
    UserComponent
  },
  methods: {
    getData(name) {
      alert(name)
    }
  },
  data() {
    return {
      users: [{
          name: 'Mukesh Kumar',
          email: 'mk.doe@example.com'
        },
        {
          name: 'Jasvant kumar',
          email: 'jks.doe@example.com'
        },
        {
          name: 'Avinash Kumar',
          email: 'akr.doe@example.com'
        },
        {
          name: 'Abhinandan',
          email: 'akp.doe@example.com'
        }
      ]
    }
  }
}
</script>
