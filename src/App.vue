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
import "devicon"

export default {
  components: {
    Home,
    NavBar,
    Top,
  },
  data() {
    return{
    }
  },
}
</script>

<style scoped>
.v-btn{
  text-transform: none
}
</style>
