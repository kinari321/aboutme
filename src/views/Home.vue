<template>
  <div align="center">
    <about-me class="odd"></about-me>
    <works class="even"></works>
    <skills class="odd"></skills>
    <contact class="even"></contact>
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

<style >
h4{
  color:grey;
}
.contents{
  padding: 3% 12%;
}
.odd{
  background-color: white;
}
.even{
  background-color: rgb(230, 230, 230);
}
</style>
