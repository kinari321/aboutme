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
          </v-avatar><br>
          <v-btn
            icon
            elevation="5"
            class="mx-3"
            href="https://github.com/kinari321"
          >
            <v-icon color="#211F1F">mdi-github</v-icon>
          </v-btn>
          <v-btn
            icon
            elevation="5"
            class="mx-3"
            href="https://twitter.com/_kinashi"
          >
            <v-icon color="#1DA1F2">mdi-twitter</v-icon>
          </v-btn>
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
              <table cellspacing=0 class="pa-2">
                <tr>
                  <td width="28%">名前</td>
                  <td>白川 生成（しらかわ きなり）</td>
                </tr>
                <tr>
                  <td>生年月日</td>
                  <td>1998年3月生まれ（23歳)</td>
                </tr>
                <tr>
                  <td style="border-style: none;">出身</td>
                  <td style="border-style: none;">和歌山県</td>
                </tr>
              </table>
              <v-list-item-title class="text-h5">
                ✍️ 学習経歴
              </v-list-item-title>
              <table cellspacing=0 class="pa-2">
                <tr>
                  <td width="28%" class="learning">2021年 1月 - 2月</td>
                  <td>Go言語・Linux・HTML/CSS・JavaScript・SQL・Git/Github</td>
                </tr>
                <tr>
                  <td class="learning">2021年 3月</td>
                  <td>AWS（VPC・EC2・RDS・IAM・Route 53・Lightsail）</td>
                </tr>
                <tr>
                  <td>2021年 4月 - 5月</td>
                  <td>ポートフォリオ制作（空き家でGo）</td>
                </tr>
                <tr>
                  <td class="learning" style="border-style: none;">2021年 6月 - 現在</td>
                  <td style="border-style: none;"> 転職活動を開始 + Docker・Github Actions(CI/CD)・Vue.jsなどを並行して学習中</td>
                </tr>
              </table>
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

<style scoped>
tr, td{
  border-bottom: 1px #000000 solid;
}
td{
  height: 30px;
}
.learning{
  height: 45px;
}
</style>