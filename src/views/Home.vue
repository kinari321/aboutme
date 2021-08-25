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
          <v-btn
              ref="button"
              block
              color="primary"
              @click="$vuetify.goTo(200, options)"
            >
            <v-icon>mdi-email-outline</v-icon>Contact
          </v-btn>
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
import * as easings from 'vuetify/lib/services/goto/easing-patterns'

export default {
  components: {
    AboutMe,
    Contact,
    ContactLinks,
    Skills,
    Works,
  },
  data() {
    return{
      type: 'number',
      number: 200,
      selector: '#scroll-with-options',
      selected: 'Button',
      elements: ['Button', 'Radio group'],
      duration: 600,
      offset: -115,
      easing: 'easeInOutCubic',
      easings: Object.keys(easings),
    }
  },
  computed: {
    target () {
      const value = this[this.type]
      if (!isNaN(value)) return Number(value)
      else return value
    },
    options () {
      return {
        duration: this.duration,
        offset: this.offset,
        easing: this.easing,
      }
    },
    element () {
      if (this.selected === 'Button') return this.$refs.button
      else if (this.selected === 'Radio group') return this.$refs.radio
      else return null
    },
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
