<template>
    <v-container>
        <div class="block GalleryBlock">
            <v-row>
                <v-col
                v-for="item in items"
                :key="item.id"
                class="d-flex child-flex"
                cols="4">
                    <v-img
                    :src="item.src"
                    :aspect-ratio="16/12"
                    class="grey lighten-2">
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
                </v-col>
            </v-row>      
        </div>
    </v-container>
</template>

<script lang="ts">
export default {
    name: 'Gallery',
    data() {
        return {
            items: [
                {
                    id: 1,
                    src: require("~/assets/images/co1.png")
                },
                {
                    id: 2,
                    src: require("~/assets/images/c1.png")
                },
                {
                    id: 3,
                    src: require("~/assets/images/c2.jpg")
                },
                {
                    id: 4,
                    src: require("~/assets/images/c3.jpg")
                },
                {
                    id: 5,
                    src: require("~/assets/images/f1.png")
                },
                {
                    id: 6,
                    src: require("~/assets/images/f2.png")
                },
                {
                    id: 7,
                    src: require("~/assets/images/s1.png")
                },
                {
                    id: 8,
                    src: require("~/assets/images/t1.png")
                },

            ]
        }
    }
}
</script>
