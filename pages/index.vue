<template>
  <div>
    <v-app>
      <AboutPage v-show="selectedTab==1"/>
      <WorkPage v-show="selectedTab==2"/>
      <ContactPage v-show="selectedTab==3"/>
      <Footer :switchInfo="switchInfo" />
    </v-app>
  </div>
</template>

<script>
import AboutPage from '~/components/pages/AboutPage.vue'
import WorkPage from '~/components/pages/WorkPage.vue'
import ContactPage from '~/components/pages/ContactPage.vue'
import Footer from '~/components/Footer.vue'

export default {
  components: {
    AboutPage,
    WorkPage,
    ContactPage,
    Footer
  },
  data() {
    return {
      title: 'ykkc-app',
      loading: false,
      selectedTab: 1
    }
  },
  methods: {
    switchInfo(value) {
      this.selectedTab = value
    }
  },
}
</script>

<style scoped>
.v-application {
  background-color: rgb(129, 156, 201);
}
</style>
