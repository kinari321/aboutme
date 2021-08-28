<template>
  <div class="contents">
    <h1 class="display-3">
      <v-icon class="display-3" style="color: black;">mdi-laptop</v-icon>
      Works
    </h1>
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
          class="my-n6 ma-10"
        ></v-img>
      </v-col>
      <v-card-text class="pa-8">
        <h2>サイト概要</h2>
        <body>
          身の回りにある空き家の写真をシェアする空き家情報サイトです。<br>
          自分が見つけた空き家を共有することで、各都道府県の空き家情報が可視化されます。
          また、自分なりの活用方法も提案することで空き家の新しい価値が想像されます。
        </body>
        <v-card-actions>
          <v-btn
            color="teamlab"
            text
            @click="show = !show"
          >
            more
          </v-btn>
          <v-spacer></v-spacer>
          <v-btn
            icon
            @click="show = !show"
          >
            <v-icon>{{ show ? 'mdi-chevron-up' : 'mdi-chevron-down' }}</v-icon>
          </v-btn>
        </v-card-actions>
        <v-expand-transition>
          <div v-show="show">
            <v-divider class="pb-5"></v-divider>
            <h3>テストユーザー</h3>
            <body>
              メールアドレス： test@example.com パスワード：test
            </body>
            <h3>開発した背景</h3>
            <body>
              2033年には空き家数2,150万戸、全住宅の3戸に1戸が空き家となる現状があります。<br>
              ただ、そんな事実を知っている人は日本に何名いらっしゃるでしょうか。
              実際、世間では空き家の問題よりも「持ち家か？賃貸か？」というテーマがよくメディアでも取り上げられています。<br>
              しかし、私はリモートワークの加速により、コロナ禍以前よりも空き家の価値が見直され、需要が高騰することで、空き家の新しい活用方法が提案される機会が訪れようとしているのではないか、と考えています。<br>
              そこで私は、空き家の新たな活用方法の提案の場 並びに 空き家の見える化 を促進したいという思いからこちらのサービスを開発しました。<br>
            </body>
            <h3>ターゲットユーザ</h3>
            <ul>
              <li>空き家を所有している持ち主の方</li>
              <li>持ち主ではないが空き家が身の回りにある方</li>
              <li>空き家を探している方</li>
              <li>空き家の活用方法を提案したい方</li>
            </ul>
            <h3>使用技術</h3>
            <table cellspacing=0 class="pa-2">
              <tr>
                <td width="27%" text class="learning font-weight-bold">バックエンド</td>
                <td>Go 1.16</td>
              </tr>
              <tr>
                <td class="learning font-weight-bold">フロントエンド</td>
                <td>Bootstrap 4.5・HTML/CSS</td>
              </tr>
              <tr>
                <td class="font-weight-bold">インフラ</td>
                <td>AWS (VPC・EC2・RDS・Route53・IAM)</td>
              </tr>
              <tr>
                <td class="font-weight-bold">CI/CD</td>
                <td>Github Actions</td>
              </tr>
              <tr>
                <td class="font-weight-bold">ミドルウェア</td>
                <td>Nginx 1.19</td>
              </tr>
              <tr>
                <td class="font-weight-bold">データベース</td>
                <td>MySQL 5.7</td>
              </tr>
              <tr>
                <td class="font-weight-bold">その他</td>
                <td>Docker (docker-compose)・Git/Github・Makefile</td>
              </tr>
            </table>
          </div>
        </v-expand-transition>
      </v-card-text>
    </v-card>

    <v-card
      cols="12"
      class="mx-auto pa-1 mt-5"
      elevation="5"
      outlined
      shaped
      align="left"
    >
      <v-card-title class="display-1">ポートフォリオサイト
        <v-btn
          icon
          elevation="1"
          class="mx-3"
          href="https://kinari-portfolio.firebaseapp.com/"
        ><v-icon color="#2e485a">mdi-open-in-new</v-icon>
        </v-btn>
        <v-btn
          icon
          elevation="1"
          href="https://github.com/kinari321/aboutme"
        ><v-icon color="#2e485a">mdi-github</v-icon>
        </v-btn>
      </v-card-title>
      <V-card-subtitle class="pt-2"><strong>制作期間：</strong>1週間</V-card-subtitle>
      <v-col cols="12">
        <v-img
          src="../assets/aboutme.png"
          class="my-n6 ma-10"
        ></v-img>
      </v-col>
      <v-card-text class="pa-8">
        <h2>サイト概要</h2>
        <body>
          ご覧いただいているこのサイトです。
        </body>
        <v-card-actions>
          <v-btn
            color="teamlab"
            text
            @click="show = !show"
          >
            more
          </v-btn>
          <v-spacer></v-spacer>
          <v-btn
            icon
            @click="show = !show"
          >
            <v-icon>{{ show ? 'mdi-chevron-up' : 'mdi-chevron-down' }}</v-icon>
          </v-btn>
        </v-card-actions>
        <v-expand-transition>
          <div v-show="show">
            <v-divider class="pb-5"></v-divider>
            <h3>使用技術</h3>
            <table cellspacing=0 class="pa-2">
              <tr>
                <td width="27%" text class="learning font-weight-bold">フロントエンド</td>
                <td class="pl-6">Vue.js 2.6</td>
              </tr>
              <tr>
                <td class="learning font-weight-bold">ホスティングサービス</td>
                <td class="pl-6">Firebase</td>
              </tr>
            </table>
          </div>
        </v-expand-transition>
      </v-card-text>
    </v-card>
  </div>
</template>

<script>
  export default {
    data: () => ({
      show: false,
    }),
  }
</script>

<style scoped>
.display-1{
  font-weight: bold;
  color: #3540d4;
}
h2, h3 {
  color: #061948;
}
body, table {
  color: rgb(31, 31, 31);
  padding: 1% 1%;
}
ul {
  color: rgb(31, 31, 31);
  padding-bottom: 8px;
  padding-top: 8px;
}
</style>