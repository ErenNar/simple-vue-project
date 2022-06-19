<template>
 
<v-container>
<section>
    <v-row justify="center" align="center" >
        <v-col cols="3" v-for="(item, index) in userList" :key="index"  class="card ma-5" >

  
        <h3 class="cart-text" >{{ item.name }}</h3>
        <p class="cart-text">{{ item.email }}</p>
          <nuxt-link class="cart-text" :to='"/"+item.id '>
            Detail...
          </nuxt-link>
        
  
        </v-col>
    </v-row>



   
     
   
</section>
</v-container>
       
      
 
          
        


         
               
              
           
       
   
  
</template>

<script>
export default {
  name: 'UserCard',
  props: {
    userList: {
      type: Array,
    },
  },
}
</script>
<style scoped lang="scss">

.card{
    background-color:#4da6ff !important;
    border-radius: 1rem !important;
    box-shadow: 5px 5px 13px 4px  rgb(0 0 0 / 67%) !important;
    color: white;
    a{
        text-decoration: none;
        color: white;
    }
      transition: .3s ease-in-out;

    &:hover{
        background-color: white !important;
        color: #4da6ff;
        a{
            color: #4da6ff;
        }
        transform: scale(1.1);
    }
}



</style>