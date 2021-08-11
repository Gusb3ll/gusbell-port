<template>
<v-img :src="avatar.src">
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
</template>

<script>
export default {
    name: 'ProfilePicture',
    data() {
        return {
            avatar: {
                src: require("~/assets/pfp.jpg")
        }
        }
    }
}
</script>
