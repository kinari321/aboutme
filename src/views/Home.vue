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
            <about-me align="center"></about-me>
            <avatar></avatar>
            <contact-links></contact-links>
          </v-sheet>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
import AboutMe from '../components/AboutMe.vue'
import Avatar from '../components/Avatar.vue'
import ContactLinks from '../components/ContactLinks.vue'

export default {
  components: {
    ContactLinks,
    Avatar,
    AboutMe,
  },
}
</script>
