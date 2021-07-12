<template>
    <v-container>
        <h1 class="v-heading text-center text-h4 text-sm-h2 text-center mb-12">About me</h1>
        <v-row justify="center">
            <v-avatar
            color="grey lighten-2"
            size="256"
            >
                <Pfp />
            </v-avatar>
        </v-row>
    </v-container>
</template>

<script lang="ts">
import Pfp from '~/components/Pfp.vue';

export default {
    head: {
        title: 'About',
    },
    components: {
        Pfp
    }
}
</script>
