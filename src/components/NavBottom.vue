<template>
<v-bottom-navigation
    v-model="value"
    :background-color="color"
    justify="center"
    class="align-self-center"
    fixed
    shift
  >
    <v-btn>
      <span>Video</span>

      <v-icon>mdi-television-play</v-icon>
    </v-btn>

    <v-btn>
      <span>Music</span>

      <v-icon>mdi-music-note</v-icon>
    </v-btn>

    <v-btn>
      <span>Book</span>

      <v-icon>mdi-book</v-icon>
    </v-btn>

    <v-btn>
      <span>Image</span>

      <v-icon>mdi-image</v-icon>
    </v-btn>
    <!-- <embed src="backsound.mp3" loop="true" autostart="true"> -->
  </v-bottom-navigation>
</template>

<script>
export default {
  data: () => ({
    file: 'backsound.mp3',
    value:1
  }),

  computed: {
    color () {
      switch (this.value) {
        case 0: return 'blue-grey'
        case 1: return 'teal'
        case 2: return 'brown'
        case 3: return 'indigo'
        default: return 'blue-grey'
      }
    }
  }
}
</script>

<style scoped>
  embed {
    height: 0;
    width: 0;
  }

</style>