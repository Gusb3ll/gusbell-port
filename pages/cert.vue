<template>
    <v-container>
        <h1 class="v-heading text-center text-h4 text-sm-h2 text-center mb-12">My Certificates</h1>
        <v-row justify="center">
            <v-btn target="_blank" text large outlined :href="'https://drive.google.com/drive/folders/11GTyAUZYb96YptMXz__C3jrC4z3onm9T?usp=sharing'"><v-icon dark>mdi-google-drive </v-icon></v-btn>
        </v-row>
        <v-main>
            <Certificate />
        </v-main>
    </v-container>
</template>
<script lang="ts">
import Certificate from '~/components/Certificate.vue';

export default {
    layout: 'default',
    head: {
    title: 'Certifications'
    },
    components: {
        Certificate
    }
}
</script>
