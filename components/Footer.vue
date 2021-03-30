<template>
  <v-footer
    color="primary lighten-1"
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
      >
        About
      </v-btn>
      <v-btn
        :disabled="loading"
        class="ma-1"
        color="black"
        plain
      >
        Work
      </v-btn>
      <v-btn
        :disabled="loading"
        class="ma-1"
        color="black"
        plain
      >
        Contact
      </v-btn>
    </v-row>
  </v-footer>
</template>

<script>
export default {
  data() {
    return {
      loading: false
    }
  }
}
</script>
