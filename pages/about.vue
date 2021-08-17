<template>
    <v-container>
        <v-row justify="center">
            <v-avatar
            color="grey lighten-2"
            size="256"
            >
                <ProfilePicture />
            </v-avatar>
        </v-row>
        <h1 class="text-center text-h5 text-sm-h4 my-12">Hi, I am Kitpipat Jaritwong. AKA, Focus.</h1>
        <v-card outlined dark class="py-4 mx-16 px-4" style="background-color: transparent">
            <p class="text-center text-sm-h6 text-h7">
                I am 17 years old, currently I am studying at Thammasat KhlongLuang Withayakhom School. 
                <br><br> 
                My dream career is to be a Front-end developer. This is because its scope of work is to make sure that the user experience is seamless and fuctional while browsing websites. I am interested in both designing and coding parts since it challenges me to utilize both arts and IT knowledge at the same time!
                <br><br>
                For the designing part, I am a visually-oriented person who loves designing with the influnece of Japanese minimal geometric design. The Japanese Minimalism has its own unique characteristics, which is well-known and being recognized across the globe. Its design gives me a sense of asymmetric, clean, warm, which I can utilize and create new templates and patterns endlessly.
                <br><br>
                Also, the coding development part allows me to translate the beautiful designs to the technical IT language, starting from selecting framework , coding interfaces, integrating responsive design, debugging software, and finally the launch for public users. 
            </p>
        </v-card>
    </v-container>
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
