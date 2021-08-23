<template>
  <v-app>
    <v-app-bar
      color="#6A76AB"
      dark
      class="text-sm-h5"
    >
      <v-tool-title>Kinari Shirakawa</v-tool-title>
      <v-spacer></v-spacer>
      <v-toolbar-items>
      <v-btn text to="/"><v-icon>mdi-account-outline</v-icon>About me</v-btn>
        <v-btn text to="/contact"><v-icon>mdi-email-outline</v-icon>Contact</v-btn>
      </v-toolbar-items>
    </v-app-bar>
    <v-main class="grey lighten-3">
      <router-view />
    </v-main>
    <v-footer color="#6A76AB" dark app>
      Footer
    </v-footer>
  </v-app>
</template>

<script>

export default {
  data() {
    return{
      drawer: null
    }
  }
};
</script>

<style scoped>
.v-btn{
  text-transform: none
}
.v-main{
  height: 1400px;
}

</style>
