<template>
  <v-container>
    <h1 class="v-heading text-center text-h4 text-sm-h2 text-center mb-4">Kitpipat Jaritwong</h1>
    <h4 class="font-weight-light text-h8 text-sm-h6 text-center mb-8">Student, Frontend Developer, Designer</h4>
    <v-row justify="center">
      <v-btn target="_blank" text large v-for="(item, i) in items" 
      :key="i" :href="item.to">{{ item.title }}</v-btn>
    </v-row>
    </v-container>
</template>

<script lang="ts">
export default {
  layout: 'default',
  head: {
    title: 'Home'
  },
  data() {
    return {
      items: [
        {
          title: "Github",
          to: "https://github.com/Gusb3ll"
        },
        {
          title: "LinkedIn",
          to: "https://Linkedin.com/in/kitpipat-jaritwong-3123a221a/"
        },
        {
          title: "Coursera",
          to: "https://www.coursera.org/user/c178abbe9febc8e12a5857fcc4ea88e2"
        },
        {
          title: "Facebook",
          to: "https://www.facebook.com/kitpipat.jaritwong/"
        },
        {
          title: "Twitter",
          to: "https://twitter.com/Gusb3ll"
        },
      ],
    };
  }
};
</script>