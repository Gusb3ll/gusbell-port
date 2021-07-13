<template>
  <v-app dark>
    <v-app-bar fixed hide-on-scroll app flat color="transparent">
      <v-tabs centered class="ml-n9" color="grey darken-1">
        <v-tab v-for="(item, i) in items" :key="i" router exact :to="item.to">
          {{ item.title }}
        </v-tab>
      </v-tabs>
    </v-app-bar>
    <v-main>
      <v-container fill-height fluid>
        <v-slide-y-transition mode="out-in">
          <Nuxt />
        </v-slide-y-transition>
      </v-container>
    </v-main>
    <v-footer padless
      color="transparent"
      v-bind="localAttrs">
      <v-spacer></v-spacer><p> {{ new Date().getFullYear() }} © Kitpipat Jaritwong</p><v-spacer></v-spacer>
    </v-footer>
  </v-app>
</template>

<script lang="ts">
export default {
  data() {
    return {
      items: [
        {
          title: "Home",
          to: "/",
        },
        {
          title: "About",
          to: "/about",
        },
        {
          title: "Projects",
          to: "/projects",
        },
        {
          title: "Certificates",
          to: "/cert",
        },
        {
          title: "Skills",
          to: "/skill",
        },
        {
          title: "Artworks",
          to: "/artworks",
        },
      ],
    };
  },
};
</script>

<style>
#app {
  background: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)), url(~assets/bg.png) !important;
  background-position: center !important;
  background-repeat: no-repeat !important;
  background-size: cover !important;
}
html, body {
  margin: 0;
  padding: 0;
}
</style>