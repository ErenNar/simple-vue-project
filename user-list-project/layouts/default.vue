<template>
  <v-app>
  <v-header>
  <VNavigate/>
  </v-header>
   
    <v-main>
     
        <Nuxt />
     
    </v-main>
   
    <v-footer  :absolute="false"  >
        <VFooter/>
    </v-footer>
  </v-app>
</template>

<script>
import VNavigate from '~/components/VNavigate.vue'
import VFooter from '~/components/VFooter.vue'
export default {
  name: 'DefaultLayout',
  

 components:{
  VNavigate,
  VFooter
 }
 
}
</script>
