<template>
    <v-container>
        <h1 class="v-heading text-center text-h4 text-sm-h2 m-n4">My Skills</h1>
        <v-main>
            <langSkill />
        </v-main>
    </v-container>
</template>

<script lang="ts">
import langSkill from '~/components/langSkill.vue';

export default {
    layout: 'default',
    head: {
        title: 'Skills'
    },
    components: {
        langSkill
    }
}
</script>