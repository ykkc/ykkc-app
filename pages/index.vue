<template>
  <section class="container">
    <div>
      <h1 class="title">
        ykkc-app
      </h1>
      <div class="links">
        <v-btn
          :disabled="loading"
          class="ma-1"
          color="grey"
          plain
        >
          About
        </v-btn>
        <v-btn
          :disabled="loading"
          class="ma-1"
          color="grey"
          plain
        >
          Work
        </v-btn>
        <v-btn
          :disabled="loading"
          class="ma-1"
          color="grey"
          plain
        >
          Contact
        </v-btn>
      </div>
    </div>
  </section>
</template>

<script>
import AppLogo from '~/components/AppLogo.vue'

export default {
  components: {
    AppLogo
  },
  data() {
    return {
      title: '',
      url: '',
      threads: [],
      loading: false,
      filter: ''
    }
  }
}
</script>

<style>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>

