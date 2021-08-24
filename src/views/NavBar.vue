<template>
  <div>
    <v-app-bar
      app
      color="#6A76AB"
      dark
      class="text-sm-h5 fixed-bar"
    >
      <v-tool-title>Kinari Shirakawa</v-tool-title>
      <v-spacer></v-spacer>
      <v-toolbar-items>
      <v-btn text to="/"><v-icon>mdi-account-outline</v-icon>About me</v-btn>
        <v-btn @click="$vuetify.goto()"><v-icon>mdi-email-outline</v-icon>Contact</v-btn>
      </v-toolbar-items>
    </v-app-bar>
  </div>
</template>

<script>
  export default {

  }
</script>

<style scoped>
.fixed-bar{
  position: sticky;
  position: -webkit-sticky;
  top: 6em;
  z-index: 100;
}
</style>