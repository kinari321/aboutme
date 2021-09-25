<template>
  <div class="px-16 py-3">
    <v-card class="my-5">
      <v-card-title class="d-flex flex-column align-start">
        <span class="title">Email</span>
      </v-card-title>
      <v-card-text class="d-flex align-center">
        <span class="email">kinari.shi21@gmail.com</span>
      </v-card-text>
    </v-card>
    <v-card class="my-5">
      <v-card-title class="d-flex flex-column align-start">
        <span class="title">Wantedly</span>
      </v-card-title>
      <v-card-text class="d-flex align-center">
        <span class="mr-1">Link:</span>
        <v-btn
          href="https://www.wantedly.com/id/kinari_shirakawa"
          text
          color="link"
          min-height="20"
          class="x-small post-link align-center py-1 px-2"
        >
          <span class="text-left">https://www.wantedly.com/id/kinari_shirakawa</span>
        </v-btn>
      </v-card-text>
    </v-card>
    <v-card class="my-5">
      <v-card-title class="d-flex flex-column align-start">
        <span class="title">Twitter</span>
      </v-card-title>
      <v-card-text class="d-flex align-center">
        <span class="mr-1">Link:</span>
        <v-btn
          href="https://twitter.com/_kinashi"
          text
          color="link"
          min-height="20"
          class="x-small post-link align-center py-1 px-2"
        >
          <span class="text-left">https://twitter.com/_kinashi</span>
        </v-btn>
      </v-card-text>
    </v-card>
    <v-card class="my-5">
      <v-card-title class="d-flex flex-column align-start">
        <span class="title">Github</span>
      </v-card-title>
      <v-card-text class="d-flex align-center">
        <span class="mr-1">Link:</span>
        <v-btn
          href="https://github.com/kinari321"
          text
          color="link"
          min-height="20"
          class="x-small post-link align-center py-1 px-2"
        >
          <span class="text-left">https://github.com/kinari321</span>
        </v-btn>
       </v-card-text>
        <v-img
          max-height="400"
          class="pt-auto ml-10 justify-center"
          src="https://grass-graph.appspot.com/images/kinari321.png"
        >
        </v-img>
    </v-card>
  </div>
</template>

<script>
  export default {

  }
</script>

<style scoped>
.title{
  color: #4f5a8a;
}
.post-link {
  display: inline-block;
  word-break: break-all;
  padding: 2px 8px;
  border-radius: 5px;
  text-transform: none !important;
  white-space: normal;
  max-width: calc(100% - 30px);
  height: inherit !important;
}
.email{
  font-weight: bold;
}
</style>