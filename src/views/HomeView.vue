<template>
    <v-app class="bg">
      <v-container style="max-width: 100%; padding:0;">
        <div class="img-container">
            <v-img src="leaf top.png"
              style="width: 700px; height: 500px; position: absolute; top: 0; right: 0;"
              max-height="500"
              min-height="650"
            ></v-img>
            <v-img src="leaf bottom.png"
              style="position: absolute; height: 500px; width:700px; left: 0; bottom: 116vh;"
              max-height="500"
              min-height="650"
            ></v-img>
            <v-img src="Frame_top.png" 
              style="position: absolute; height: 91px; width:91px; margin-left: 17em; margin-top: 5em"
            ></v-img>
            <v-img src="Frame_bottom.png"
            style="position: absolute; height: 91px; width:91px; margin-left: 69em; margin-top: 32em"
            ></v-img>
            <div class="wrapper"> 
              <h1>Ega Frandika, B.Sc.IT</h1>
              <p>&</p>
              <h2>Tri Ega Septiana, S.Kep,Ners</h2>
            </div>
        </div>
            <NavBar />
            <NavBottom />
            <Body />
      </v-container>
    </v-app>
</template>

<script>
import NavBar from '@/components/NavBar.vue';
import NavBottom from '@/components/NavBottom.vue';
import Body from '@/components/Body.vue';

  export default {
    name: 'Home',

    components: {
    NavBar,
    NavBottom,
    Body
}
}
</script>

<style scoped>
  .bg {
    background: url('../assets/bg.jpeg') no-repeat center fixed !important;
    overflow: hidden;
    overflow-x: hidden;
  } 

  h1 {
    display: block;
    font-family: cursive;
    font-size: 60px;
    left: 8em;
    top: 4em;
  }

  h2 {
    display: block;
    font-family: cursive;
    font-size: 60px;
    left: 11em;
    top: 6.5em;
  }

  p {
    display: block;
    font-family: cursive;
    font-size: 60px;
    left: 12em;
    top: 5.3em;
  }

  .wrapper {
    align-content: center;
    text-align: center;
    position: absolute;
    top: 30vh;
    left: 46vh;
  }
</style>
