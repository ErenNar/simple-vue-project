<template>
      <nav>
     <v-container>
        <v-row justify="center">
          <v-col cols="12">
              <h2 class="text-center"> <nuxt-link to="/" active-class="link">User List</nuxt-link> </h2>
              <hr color="white">
          </v-col>
        </v-row>

      </v-container>
      </nav>
</template>

<script>
export default {
name:"VNavigate"
}
</script>
<style scoped>

nav{
  background-color: black;
}

.link{
  color: white;
  text-decoration: none;
}
</style>

