<template>
  <v-app>
    <NavBar />
    <Top />
    <v-main>
      <Home />
    </v-main>
  </v-app>
</template>

<script>
import Home from '@/views/Home.vue'
import NavBar from '@/views/NavBar.vue'
import Top from '@/components/Top.vue'

export default {
  components: {
    Home,
    NavBar,
    Top,
  },
  data() {
    return{
      drawer: null,
    }
  },
}
</script>

<style scoped>
.v-btn{
  text-transform: none
}
.v-main{
  height: 1400px;
  /* background-color: aquamarine; */
}
</style>
