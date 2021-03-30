<template>
  <div>
    <v-app>
      <AboutPage/>
      <Footer/>
    </v-app>
  </div>
</template>

<script>
import AboutPage from '~/components/pages/AboutPage.vue'
import Footer from '~/components/Footer.vue'

export default {
  components: {
    AboutPage,
    Footer
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
