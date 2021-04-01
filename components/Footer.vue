<template>
  <v-footer
    color="secondary darken-1"
    padless
  >
    <v-row
      justify="center"
      no-gutters
    >
      <v-btn
        :disabled="loading"
        class="ma-1"
        color="black"
        plain
        @click="switchInfo(1)"
      >
        About
      </v-btn>
      <v-btn
        :disabled="loading"
        class="ma-1"
        color="black"
        plain
        @click="switchInfo(2)"
      >
        Works
      </v-btn>
      <v-btn
        :disabled="loading"
        class="ma-1"
        color="black"
        plain
        @click="switchInfo(3)"
      >
        Contact
      </v-btn>
      <v-col
        class="secondary darken-1 py-2 text-center black--text"
        cols="12"
      >
        <div class="copy-right">
          &copy;ykkc
        </div>
      </v-col>
    </v-row>
  </v-footer>
</template>

<script>
export default {
  data() {
    return {
      loading: false
    }
  },
  props: {
    switchInfo: Function
  }
}
</script>
