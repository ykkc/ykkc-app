<template>
  <v-main>
    <v-card
      class="mx-auto mt-8 pa-4"
      max-width="400"
      rounded
      outlined
    > 
      <div class="text-h5 text-center font-weight-bold pb-4">
        Profile
      </div>
      <v-list-item>
        <v-avatar
          class="mx-auto"
          size="200"
        >
          <img
            src="../../assets/icon_ykkc.jpg"
            alt="ykkc"
          >
        </v-avatar>
      </v-list-item>
      <div class="text-center font-weight-bold mt-4">
        ykkc
      </div>
    </v-card>
    <v-card
      class="mx-auto mt-4 pa-4"
      max-width="400"
      rounded
      outlined
    > 
      <div class="text-h5 text-center font-weight-bold pb-4">
        SNS
      </div>
      <v-list-item>
        <v-btn
          class="mx-auto"
          outlined
          @click="openTwitter"
        >
          Twitter
        </v-btn>
        <v-btn
          class="mx-auto"
          outlined
          @click="openFacebook"
        >
          Facebook
        </v-btn>
        <v-btn
          class="mx-auto"
          outlined
          @click="openGitHub"
        >
          GitHub
        </v-btn>
      </v-list-item>
    </v-card>
    <v-card
      class="mx-auto mt-4 pa-4"
      max-width="400"
      rounded
      outlined
    > 
      <div class="text-h5 text-center font-weight-bold pb-4">
        Working at
      </div>
      <div class="text-h6 text-center font-weight-bold">
        Main
      </div>
      <CompanyCard
        name="hey, Inc."
        period="2019/02 -"
        role="iOS Developer"
      />
      <div class="text-h6 text-center font-weight-bold mt-4">
        Side
      </div>
      <CompanyCard
        name="Lang-8, Inc."
        period="2020/07 -"
        role="iOS Developer"
      />
    </v-card>
    <v-card
      class="mx-auto mt-4 mb-8 pa-4"
      max-width="400"
      rounded
      outlined
    > 
      <div class="text-h5 text-center font-weight-bold pb-4">
        History
      </div>
      <div class="text-h6 text-center font-weight-bold mt-4">
        Main
      </div>
      <CompanyCard
        name="SOELU, Inc."
        period="2016/09 - 2019/01"
        role="Software Developer"
      />
      <CompanyCard
        name="YAZ CO.,LTD."
        period="2015/04 - 2016/08"
        role="Software Developer"
      >
        <ul>
          <li>
            iOS Application x 3
          </li>
          <li>
            Android Application x 2
          </li>
          <li>
            Windows Application x 1
          </li>
          <li>
            Driver for BLE Device x 1
          </li>
          <li>
            Backend system for desktop robot control x 1
          </li>
        </ul>
      </CompanyCard>
      <div class="text-h6 text-center font-weight-bold mt-4">
        Side
      </div>
      <CompanyCard
        name="A certain company"
        period="2019/10 - 2020/01"
        role="Software Developer"
      />
      <CompanyCard
        name="SOELU, Inc."
        period="2016/05 - 2016/08"
        role="Software Developer"
      />
    </v-card>
  </v-main>
</template>

<script>
import CompanyCard from '~/components/organisms/CompanyCard.vue'

export default {
  data() {
    return {
      loading: false
    }
  },
  methods: {
    openTwitter () {
      window.open("https://twitter.com/_ykkc", '_blank')
    },
    openFacebook () {
      window.open("https://www.facebook.com/ylane.admirable", '_blank')
    },
    openGitHub () {
      window.open("https://github.com/ykkc", '_blank')
    }
  },
  components: {
    CompanyCard
  }
}
</script>
