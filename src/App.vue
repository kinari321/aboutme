<template>
  <v-app>
    <v-navigation-drawer app v-model="drawer" clipped>Navigation Lists</v-navigation-drawer>
    <v-app-bar color="primary" dark app clipped-left>
      <v-app-bar-nav-icon @click="drawer=!drawer"></v-app-bar-nav-icon>
      <v-tool-title>Nav Bar</v-tool-title>
      <v-spacer></v-spacer>
      <v-toolbar-items>
      <v-btn text>About me</v-btn>
        <v-btn text>Contact</v-btn>
      </v-toolbar-items>
    </v-app-bar>
    <v-footer color="primary" dark app>
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
</style>
