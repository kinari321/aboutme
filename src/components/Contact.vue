<template>
  <div>
    <h1>Contact</h1>
    <div class="subtitle">ご連絡</div>
    <v-sheet
      class="px-15 pt-10 contacts"
    >
      <v-avatar size="150">
        <img
          src="../assets/kinari.png"
          alt="Kinari"
        >
      </v-avatar>
      <span class="ma-8 arrow_box">
        🙆‍♂️ 現在転職活動中です！
        📩 お気軽にメッセージください！
      </span>
      <contact-links />
    </v-sheet>
  </div>

</template>

<script>
import ContactLinks from './ContactLinks.vue'

export default {
  components: { ContactLinks },
}
</script>

<style scoped>
.arrow_box{
    position:relative;
    width:300px;
    height:140px;
    background:#f0f0f0;
    padding:20px;
    text-align:left;
    color:#333333;
    font-size:14px;
    font-weight:bold;
    border-radius:15px;
    -webkit-border-radius:15px;
    -moz-border-radius:15px;
}
.arrow_box:after{
    border: solid transparent;
    content:'';
    height:0;
    width:0;
    pointer-events:none;
    position:absolute;
    border-color: rgba(230, 230, 230, 0);
    border-top-width:10px;
    border-bottom-width:10px;
    border-left-width:30px;
    border-right-width:30px;
    margin-top: -10px;
    border-right-color:#f0f0f0;
    right:100%;
    top:60%;
}

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
.contacts{
  background-color: grey;
}
</style>