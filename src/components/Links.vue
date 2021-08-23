<template>
  <div class="px-10 py-5">

    <v-card class="my-5">
      <v-card-title class="d-flex flex-column align-start">
        <span class="title">ポートフォリオ：空き家でGo</span>
      </v-card-title>
      <v-card-text class="d-flex align-center">
        <span class="mr-1">Link1:</span>
        <v-btn
          href="http://akiyadego.com/"
          text
          color="link"
          min-height="20"
          class="x-small post-link align-center py-1 px-2"
        >
          <span class="text-left">http://akiyadego.com/</span>
        </v-btn>
      </v-card-text>
      <v-card-text class="d-flex align-center mt-n5">
        <span class="mr-1">Link2:</span>
        <v-btn
          href="https://github.com/kinari321/AkiyaDeGo"
          text
          color="link"
          min-height="20"
          class="x-small post-link align-center py-1 px-2"
        >
          <span class="text-left">https://github.com/kinari321/AkiyaDeGo</span>
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
    </v-card>

    <v-card class="my-5">
      <v-card-title class="d-flex flex-column align-start">
        <span class="title">Zenn</span>
      </v-card-title>
      <v-card-text class="d-flex align-center">
        <span class="mr-1">Link:</span>
        <v-btn
          href="https://zenn.dev/kinariru"
          text
          color="link"
          min-height="20"
          class="x-small post-link align-center py-1 px-2"
        >
          <span class="text-left">https://zenn.dev/kinariru</span>
        </v-btn>
      </v-card-text>
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