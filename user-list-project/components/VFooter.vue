<template>
<footer>

      <v-container>
        <v-row justify="center">
          <v-col cols="12">
          <p class="text-center pa-0 ma-0">&copy; {{ new Date().getFullYear() }}</p>
          </v-col>
        </v-row>
      </v-container>
</footer>
</template>

<script>
export default {
name:"VFooter"
}
</script>

<style  scoped>
footer{
    background-color: black;
    color: white;
}
</style>