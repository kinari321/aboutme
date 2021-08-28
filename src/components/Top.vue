<template>
  <div>
    <v-container
      app
      fluid
      fill-height
      class="background-image"
    >
      <v-row>
        <v-col
        class="background-image-text">
          <p>Welcome to my website!</p>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
  export default {

  }
</script>

<style scoped>
.background-image{
  background: url("../assets/teamlab-min.png");
  background-size: cover;
  background-position: center center;
  width: 100%;
  height: 90vh;
}
.background-image-text{
  color: aliceblue;
  text-align: center;
  font-size: 28px;
}


</style>