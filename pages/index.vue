<template>
  <div>
    <v-app>
      <MainPage />
      <Footer />
    </v-app>
  </div>
</template>

<script>
import MainPage from '~/components/pages/MainPage.vue'
import Footer from '~/components/Footer.vue'

export default {
  components: {
    MainPage,
    Footer
  },
  data() {
    return {
      title: 'ykkc-app',
      loading: false
    }
  },
}
</script>

<style scoped>
.v-application {
  background-color: rgb(129, 156, 201);
}
</style>
