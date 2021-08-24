<template>
  <v-app>
    <v-app-bar
      color="#6A76AB"
      dark
      class="text-sm-h5 "
    >
      <v-tool-title>Kinari Shirakawa</v-tool-title>
      <v-spacer></v-spacer>
      <v-toolbar-items>
      <v-btn text to="/"><v-icon>mdi-account-outline</v-icon>About me</v-btn>
        <v-btn text to="/contact"><v-icon>mdi-email-outline</v-icon>Contact</v-btn>
      </v-toolbar-items>
    </v-app-bar>
    <v-main absolute class="grey lighten-3">
      <Home></Home>
    </v-main>
  </v-app>
</template>

<script>
import Home from '@/views/Home.vue'

export default {
  components: {
    Home,
  },
  data() {
    return{
      drawer: null
    }
  }
};
</script>

<style scoped>
.v-app-bar{
  position: sticky;
  top: 0;
  z-index: 100;
}
.v-btn{
  text-transform: none
}
.v-main{
  height: 1400px;
}

</style>
