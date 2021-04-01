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
        @click="goAboutPage"
      >
        About
      </v-btn>
      <v-btn
        :disabled="loading"
        class="ma-1"
        color="black"
        plain
        @click="goWorksPage"
      >
        Works
      </v-btn>
      <v-btn
        :disabled="loading"
        class="ma-1"
        color="black"
        plain
        @click="goContactPage"
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
  methods: {
      goAboutPage() {
          this.$router.push('/about')
      },
      goWorksPage() {
          this.$router.push('/works')
      },
      goContactPage() {
          this.$router.push('/contact')
      }
  },
}
</script>
