<template >
  <v-container>
    <v-row justify="start" align="center">
    
     
        <v-col cols="12">
          <user-detail :detailUser="detailUser"></user-detail>
        </v-col>
     

     
    </v-row>
   
  </v-container>
</template>

<script>
import UserDetail from "@/components/UserDetail.vue";
export default {
naem:"Detail",
  components:{
    UserDetail
  },
  async asyncData({ $axios , params  }) {
    try {
      const BaseURL = 'https://jsonplaceholder.typicode.com/users/'+ params.slug
      const detail = await $axios.$get(BaseURL)
      console.log(detail);
     return{
        detailUser:detail      
     }
    } catch (error) {
      console.log(error)
    }
  },

}
</script>

