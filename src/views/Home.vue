<template>
  <div>
    <v-container>
      <v-row>
        <v-col
          cols="12"
          sm="1"
        >
          <v-sheet
            rounded="lg"
            min-height="268"
            class="grey lighten-3"
          >
            <!--  -->
          </v-sheet>
        </v-col>

        <v-col
          cols="12"
          sm="8"
        >
          <v-sheet
            min-height="70vh"
            rounded="lg"
          >
            <Links></Links>
          </v-sheet>
        </v-col>

        <v-col
          cols="12"
          sm="3"
        >
          <v-sheet
            rounded="lg"
            min-height="268"
          >
            <!--  -->
          </v-sheet>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
import Links from '../components/Links.vue'

export default {
  components: {
    Links,
  },
}
</script>
