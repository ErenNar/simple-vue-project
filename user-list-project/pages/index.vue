<template>
 
   

    <user-card :userList="userList"></user-card>
    

</template>

<script>
import UserCard from '~/components/UserCard.vue'
export default {
  name: 'IndexPage',

  async asyncData({ $axios }) {
    try {
      const BaseURL = 'https://jsonplaceholder.typicode.com/users'
      const users = await $axios.$get(BaseURL)
      return { userList: users }
    } catch (error) {
      console.log(error)
    }
  },

  components: {
    UserCard,
  },
}
</script>
