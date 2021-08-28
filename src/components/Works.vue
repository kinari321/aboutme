<template>
  <div class="contents">
    <h1 class="display-3">Works</h1>
    <div class="">制作物</div>
    <v-card
      cols="12"
      class="mx-auto pa-1 mt-5"
      elevation="5"
      outlined
      shaped
      align="left"
    >
      <v-card-title class="display-1">空き家でGo
        <v-btn
          icon
          elevation="1"
          class="mx-3"
          href="http://akiyadego.com/"
        ><v-icon color="#2e485a">mdi-open-in-new</v-icon>
        </v-btn>
        <v-btn
          icon
          elevation="1"
          class="mx-"
          href="https://github.com/kinari321/AkiyaDeGo"
        ><v-icon color="#2e485a">mdi-github</v-icon>
        </v-btn>
      </v-card-title>
      <V-card-subtitle class="pt-2"><strong>制作期間：</strong>約3ヶ月</V-card-subtitle>
      <v-col cols="12">
        <v-img
          src="../assets/AkiyaDeGo.gif"
          class="my-n6"
        ></v-img>
      </v-col>
      <v-card-text>あああ</v-card-text>
    </v-card>
    <v-card
      cols="12"
      class="mx-auto mt-5"
      elevation="5"
      outlined
      shaped
    >
      <v-card-title >タイトル</v-card-title>
      <V-card-subtitle>サブタイトル</V-card-subtitle>
      <v-card-text>本文</v-card-text>
    </v-card>
  </div>
</template>

<script>
  export default {

  }
</script>

<style scoped>
.display-1{
  font-weight: bold;
  color: #3c47eb;
}
</style>