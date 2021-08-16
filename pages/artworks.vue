<template>
    <v-container>
        <h1 class="v-heading text-center text-h4 text-sm-h2 mb-12">My Artworks</h1>
        <Artwork />
    </v-container>
</template>

<script>
import Artwork from '~/components/Artwork.vue';

export default {

    head: {
        title: 'Artworks',
    },
    components: {
        Artwork
    }
}
</script>
