<template>
    <v-container>
        <h1 class="v-heading text-center text-h4 text-sm-h2 mb-12">My Projects</h1>
        <Project />
    </v-container>
</template>

<script lang="ts">
import Project from '~/components/Project.vue'

export default {
    layout: 'default',
    head: {
        title: 'Projects'
    },
    components: {
        Project
    }
}
</script>