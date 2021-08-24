<template>
  <v-app>
    <NavBar></NavBar>
    <v-main absolute class="grey lighten-3">
      <Home></Home>
    </v-main>
  </v-app>
</template>

<script>
import Home from '@/views/Home.vue'
import NavBar from '@/views/NavBar.vue'

export default {
  components: {
    Home,
    NavBar,
  },
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
