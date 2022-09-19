<template>
  <v-app class="body-container">
    <div class="text">
      <h1>SAVE THE DATE</h1>
    </div>
      <Countdown class="count-down" end="September 20, 2022">
      </Countdown>
  </v-app>
</template>

<script>
import Countdown from 'vuejs-countdown'
export default {
  components: { Countdown }
}
</script>

<style scoped>
  .count-down {
    text-align: center;
    align-content: center;
    font-display: relative;
    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    margin-top: 40px;
    margin-bottom: 40px;
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

  h1 {
    font-family: Arial, Helvetica, sans-serif;
    text-align: center;
    justify-content: center;
    align-content: center;
    margin: 0;
    width: 100%;
    margin-top: 50px;
  }
  p {
    align-content: center;
    font-size: 20px;
  }
</style>