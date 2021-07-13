<template>
    <v-container>
        <!-- <h1 class="v-heading text-center text-h4 text-sm-h2 mb-12">About me</h1> -->
        <v-row justify="center">
            <v-avatar
            color="grey lighten-2"
            size="256"
            >
                <Pfp />
            </v-avatar>
        </v-row>
        <v-main class="d-flex wrap">
            <h1 class="text-center text-h5 text-sm-h3 pb-8">Hi, I am Kitpipat Jaritwong</h1>
            <v-card outlined dark class="px-4 py-4" style="background-color: transparent">
                <p class="text-center text-sm-h5 text-h7">I am 17 years old, and I studied at Thammasat KhlongLuang Withayakhom school. <br><br> 
                I usually play game like "osu" and "Apex Legend" and others. I love about coding and designing "furturistic" UI and others stuff <br><br>
                I also love about Japanese related stuff, especially anime and manga.
                </p>
            </v-card>
        </v-main>
    </v-container>
</template>

<script lang="ts">
import Pfp from '~/components/Pfp.vue';

export default {
    layout: 'default',
    head: {
        title: 'About',
    },
    components: {
        Pfp
    }
}
</script>
