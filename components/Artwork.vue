<template>
    <v-container>
        <v-row justify="center" 
        v-for="image in images" 
        :key="image.id" class="mb-8">
            <v-card outlined dark class="px-4 pb-4" style="background-color: transparent">
                <v-card-title class="text-sm-h5 text-h7"> {{ image.title }} </v-card-title>
                <v-img :src="image.src" contain :max-width="image.width" :max-height="image.height">
                    <template v-slot:placeholder>
                        <v-row
                        class="fill-height ma-0"
                        align="center"
                        justify="center">
                            <v-progress-circular
                            indeterminate
                            color="grey lighten-5">
                            </v-progress-circular>
                        </v-row>
                    </template>
                </v-img>
            </v-card>
        </v-row>
    </v-container>
</template>

<script lang="ts">
export default {
    name: 'Artwork',
    data() {
        return {
            images: [
                {
                    id: 1,
                    width: "610",
                    height: "180",
                    title: "Github banner",
                    src: require("~/assets/artwork/github-banner.png"),
                },
                {
                    id: 2,
                    width: "640",
                    height: "180",
                    title: "guweb banner",
                    src: require("~/assets/artwork/guweb-banner-2.png"),
                },
                {
                    id: 3,
                    width: "640",
                    height: "360",
                    title: "guweb banner-old",
                    src: require("~/assets/artwork/guweb-banner.png"),
                },
            ]
        }
    }
}
</script>
