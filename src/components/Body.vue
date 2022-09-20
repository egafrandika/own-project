<template>
  <v-app class="body-container">
    <div class="body-divider">
      <img src="divider.png">
    </div>
    <div class="wedding-text">
      <h1>SAVE <span>THE</span> DATE</h1>
      <div class="wedding-date">
        <h1>SEP | 27 | 2017</h1>
      </div>
    </div>
    <Countdown class="count-down" end="September 24, 2022" />
    <div class="ring">
      <img src="ring.png">
      <div class="img-border">
        <img src="woman.jpeg">
        <img src="man.jpeg">  
      </div>
    </div>
  </v-app>
</template>

<script>
import Countdown from 'vuejs-countdown'
export default {
  components: { Countdown },
}
</script>

<style scoped>
  .ring img {
    position: relative;
    top: 100px;
    width: 200px;
    height: 200px;
  }
  .wedding-text h1 {  
    font-family: 'Times New Roman', Times, serif;
    font-style: italic;
  }

  .wedding-date h1 {
    font-size: 50px;
    font-family: 'Times New Roman', Times, serif;
    font-style: normal !important;
  }

  .body-divider img {
    align-content: center;
    width: 100%;
    height: 80px;
    transform: scaleY(-1);
  }

  .img-border {
    width: 100%;
    position: absolute;
    top: 5em;
  }

  .img-border img {
    border-radius: 50%;
    margin-top: 5vh;
    margin-left: 16em;
    margin-right: 16em;
  }

  .count-down {
    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    margin-right: 2.6vh;
  }

  .card-rundown {
    justify-content: center;
    display: flex;
    flex-direction: row;
  }

  .body-container {
    min-height: 200vh;
    top: 83.5vh;
    background-color: beige;
    text-align: center;
    position: relative;
  }

  .card {
    margin: 10px 20px 10px 20px;
    padding: 20px;
    background-color: violet;
    border-top-right-radius: 15px;
    border-bottom-left-radius: 15px;
  }

  span {
    font-family: Verdana, Geneva, Tahoma, sans-serif;
    font-style: normal !important;
  }
  p {
    align-content: center;
  }
</style>