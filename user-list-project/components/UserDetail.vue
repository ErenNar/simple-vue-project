<template>
      <div   class="detail">
          <v-row>
            <v-col>


            <h4 >   <v-icon color="#00ccff"> mdi-account </v-icon>: {{detailUser.name}} </h4>
           
            </v-col>
            <v-col>
            <p>  <v-icon  color="#00ccff" small> mdi-at </v-icon>:   {{detailUser.email}}</p>
          
                  <p> <v-icon  color="#00ccff" small> mdi-cellphone </v-icon>: {{detailUser.phone}}</p>
                 <p> <v-icon  color="#00ccff" small> mdi-web </v-icon>: {{detailUser.website}}</p>
                  <p>

                 <v-icon  color="#00ccff" small> mdi-map-marker </v-icon> :
                 <pre>
                  <v-icon  color="#00ccff" small> mdi-google-street-view </v-icon>:{{detailUser.address.street}}
                  <v-icon  color="#00ccff" small> mdi-home </v-icon>:{{detailUser.address.suite}}
                  <v-icon  color="#00ccff" small> mdi-city </v-icon>:{{detailUser.address.city}}
                 </pre>
                  </p>
                  
                      
               
        
                  
               
                
            </v-col>
           
          </v-row>
            </div>
</template>

<script>
export default {
name:'UserDetail',
props:{
    detailUser:{
        type:Object,

    }
}
}
</script>

<style scoped>

.detail{
    border-bottom:1px solid black;
    padding: 2rem;
}

</style>
