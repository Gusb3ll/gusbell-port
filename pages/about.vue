<template>
    <div>
        <v-row justify="center">
            <v-avatar
            color="grey lighten-2"
            size="256"
            >
                <ProfilePicture />
            </v-avatar>
        </v-row>
        <v-main class="d-flex wrap">
            <h1 class="text-center text-h5 text-sm-h3 pb-8">Hi, I am Kitpipat Jaritwong</h1>
            <v-card outlined dark class="px-16 py-4 mx-16" style="background-color: transparent">
                <p class="mx-16 text-center text-sm-h5 text-h7">I am 17 years old, and I am currently studying at Thammasat KhlongLuang Withayakhom School. <br><br> 
                I am very interested in coding and designing, for the coding part I mainly does the frontend part and sometimes does the backend part, for the
                designing part, I love designing 'futuristic' looking design as shown on my artwork page. <br><br>
                I am also interested in japanese culture and their design, most of my design are mostly reference from japanese design. I also love their manga, 
                anime as well.
                </p>
            </v-card>
        </v-main>
    </div>
</template>

<script lang="ts">
import ProfilePicture from '~/components/ProfilePicture.vue';

export default {
    layout: 'default',
    head: {
        title: 'About',
    },
    components: {
        ProfilePicture
    }
}
</script>
