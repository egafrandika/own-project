<template>
    <v-row justify="center">
      <v-col cols="12" class="text-center">
        <div class="nav">
          <v-btn class="button" text @click="scroll('home')">Home</v-btn>
          <v-btn class="button" text @click="scroll('event')">OUR STORY</v-btn>
          <v-btn class="button" text @click="scroll('location')">WEDDING PARTY</v-btn>
          <v-btn class="button" text @click="scroll('invitaiton')">GALLERY</v-btn>
        </div>
      </v-col>
    </v-row>
</template>
<script>

export default {

}

</script>

<style scoped>
  
.v-row {
  min-height: initial;
}

.nav {
  position: relative;
  width: 100%;
  bottom: -8em;
}

.button {
  margin: 1.5em;
  padding: 0.5em;
}

@media only screen and (max-width: 375px) {

  .nav {
    bottom: -5em;
  }
  
  .button {
    font-size: 9px;
    justify-content: flex-end;
    padding: 0;
    margin: 0;
  }
  
}
</style>