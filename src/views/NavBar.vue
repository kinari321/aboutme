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
      <v-btn
        ref="button"
        color="#6A76AB"
        @click="$vuetify.goTo(50, options)"
      >
      <v-icon>mdi-account-outline</v-icon>About Me
      </v-btn>
      <v-btn
          ref="button"
          color="#6A76AB"
          @click="$vuetify.goTo(200, options)"
        >
        <v-icon>mdi-email-outline</v-icon>Contact
      </v-btn>
      </v-toolbar-items>
    </v-app-bar>
  </div>
</template>

<script>
import * as easings from 'vuetify/lib/services/goto/easing-patterns'


export default {
  data() {
    return{
      type: 'number',
      number: 200,
      selector: '#scroll-with-options',
      selected: 'Button',
      elements: ['Button', 'Radio group'],
      duration: 500,
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

<style scoped>
.fixed-bar{
  position: sticky;
  position: -webkit-sticky;
  top: 6em;
  z-index: 100;
}
</style>