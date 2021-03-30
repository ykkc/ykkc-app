<template>
  <div>
    <Footer/>
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
      title: '',
      url: '',
      threads: [],
      loading: false,
      filter: ''
    }
  }
}
</script>
