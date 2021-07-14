<template>
  <v-container>
    <h1 class="v-heading text-center text-h4 text-sm-h2 mb-12">
      Extra Information
    </h1>
    <v-row
      v-for="extra in extras"
      :key="extra.id"
      justify="center"
      class="mb-8"
    >
      <v-card
        outlined
        dark
        class="px-4 pb-4"
        style="background-color: transparent"
      >
        <v-card-title class="text-sm-h5 text-h7">
          {{ extra.title }}
        </v-card-title>
        <v-card-text class="pt-2">
          <v-row justify="center">
            <a :href="extra.to" style="text-decoration: none"><h1>{{ extra.description }}</h1></a>
          </v-row>
        </v-card-text>
      </v-card>
    </v-row>
  </v-container>
</template>

<script lang="ts">
export default {
  layout: "default",
  head: {
    title: "Extra",
  },
  data() {
    return {
      extras: [
        {
          id: "1",
          title: "Development Framework",
          description: "Nuxt.js + Vuetify",
          to: "https://nuxtjs.org"
        },
        {
          id: "2",
          title: "Background Reference",
          description: "キョウノミヤコ",
          to: "https://alt.hololive.tv/holonometria/location/kyo-no-miyako/"
        },
      ],
    };
  },
};
</script>
