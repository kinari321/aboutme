<template>
  <div>
    <about-me align="center" style="height: 200px; background-color: white;"></about-me>
    <works align="center" style="height: 200px; background-color: grey;"></works>
    <skills align="center" style="height: 200px; background-color: white;"></skills>
    <contact align="center" style="height: 200px; background-color: grey;" ></contact>
  </div>
</template>

<script>
import AboutMe from '../components/AboutMe.vue'
import Contact from '../components/Contact.vue'
import Skills from '../components/Skills.vue'
import Works from '../components/Works.vue'
import * as easings from 'vuetify/lib/services/goto/easing-patterns'

export default {
  components: {
    AboutMe,
    Contact,
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
