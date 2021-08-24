<template>
  <div>
    <v-container>
      <v-row justify="center">
        <v-col
          cols="12"
          sm="9"
        >
          <v-sheet
            min-height="70vh"
            rounded="lg"
          >
            <about-me align="center" style="height: 200px; background-color: yellow;"></about-me>
            <works align="center" style="height: 200px; background-color: green;"></works>
            <skills align="center" style="height: 200px; background-color: red;"></skills>
            <contact align="center" style="height: 200px;" ></contact>
            <contact-links style="background-color: blue;"></contact-links>
          </v-sheet>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
import AboutMe from '../components/AboutMe.vue'
import Contact from '../components/Contact.vue'
import ContactLinks from '../components/ContactLinks.vue'
import Skills from '../components/Skills.vue'
import Works from '../components/Works.vue'

export default {
  components: {
    AboutMe,
    Contact,
    ContactLinks,
    Skills,
    Works,
  },
}
</script>

<style>
.subtitle{
  color: #757d9b;
}
h4{
  color:grey
}
</style>
