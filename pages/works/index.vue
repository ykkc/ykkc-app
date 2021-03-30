<template>
  <div>
    <v-app>
      <v-main>
        Works Page
      </v-main>
      <Footer/>
    </v-app>
  </div>
</template>

<script>
import Footer from '~/components/Footer.vue'

export default {
  components: {
    Footer
  },
  data() {
    return {
      title: 'About',
      loading: false
    }
  }
}
</script>
