<template>
  <div class=contents>
    <h1 class="display-3">
      <v-icon class="display-3" style="color: black;">mdi-account-outline</v-icon>
      About me
    </h1>
    <div class="pb-7">私について</div>
      <v-row
      align="end"
      class="fill-height"
      >
        <v-col
          align-self="start"
          class="pa-0"
          cols="5"
        >
        <v-avatar size="250">
          <img
            src="../assets/kinari.png"
            alt="Kinari"
          >
        </v-avatar>
        </v-col>
        <v-col
          align-self="start"
          align="left"
          class="pa-0"
          cols="7"
        >
          <v-list-item>
            <v-list-item-content>
              <v-list-item-title class="text-h5">
                👨‍💻 プロフィール
              </v-list-item-title>
              <v-list-item>
                白川 生成
                1998年3月生まれ（23歳）
                和歌山県出身
              </v-list-item>
              <v-list-item-title class="text-h5">
                ✍️ 学習経歴
              </v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </v-col>
      </v-row>
  </div>
</template>

<script>
  export default {

  }
</script>

<style lang="scss" scoped>

</style>