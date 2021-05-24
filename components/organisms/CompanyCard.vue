<template>
  <v-card
      class="mt-4"
      max-width="400"
      rounded
      outlined
    >
      <v-list-item>
        <v-list-item-content>
          <v-list-item-title>
            {{ name }}
          </v-list-item-title>
          <v-list-item-subtitle>
            {{ period }}
          </v-list-item-subtitle>
          <v-list-item-subtitle>
            {{ role }}
          </v-list-item-subtitle>
          <v-list-item-subtitle>
            <slot />
          </v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>
  </v-card>
</template>

<script>
export default {
  data() {
    return {
      loading: false
    }
  },
  props: {
    name: String,
    period: String,
    role: String
  },
}
</script>
