<template>
<v-row>
    <v-col
        v-for="project in projects"
        :key="project.id"
        class="d-flex child-flex"
        cols="4"
    >
        <v-card
            elevation="2"
            outlined
            shaped
            dark
            style="background-color: rgba(0, 0, 0, 0.2)"
        >
            <v-card-title> {{ project.name }} </v-card-title>
            <v-card-subtitle> {{ project.sub }} </v-card-subtitle>
            <v-card-text> {{ project.desc }} </v-card-text>
            <v-card-actions>
                <v-btn
                    v-if="project.to"
                    style="background-color: transparent"
                    :href="project.to"
                    >
                    <v-icon>mdi-github</v-icon>
                </v-btn>
                <v-btn
                    v-if="project.to2"
                    style="background-color: transparent"
                    :href="project.to2"
                >
                    <v-icon>mdi-earth</v-icon>
                </v-btn>
            </v-card-actions>
        </v-card>
    </v-col>
</v-row>
</template>

<script>
export default {
    name: "Project",
    data() {
        return {
            projects: [
                {
                    id: 1,
                    name: "oturna (Private)",
                    sub: "Frontend/Backend",
                    desc: "A tournament manager for rhythm game, osu!",
                    to: "",
                    to2: "https://omthpl.varkaria.tech",
                },
                {
                    id: 2,
                    name: "guweb",
                    sub: "Frontend/Backend",
                    desc: "Front-facing appearance of the osu! server protocol.",
                    to: "https://github.com/Varkaria/guweb/tree/admin-panel",
                },
                {
                    id: 3,
                    name: "Sayuka",
                    sub: "Frontend",
                    desc: "A dojin reading website for Thailand community.",
                    to: "https://github.com/Varkaria/sayuka",
                    to2: "https://sayuka.vercel.app",
                },
                {
                    id: 4,
                    name: "Holotranslator",
                    sub: "Author",
                    desc: "Live Japanese speech to text translator.",
                    to: "https://github.com/Gusb3ll/Holotranslator",
                },
                {
                    id: 5,
                    name: "Euler-bot",
                    sub: "Author",
                    desc: "A bot for mathmetic POSN discord.",
                    to: "https://github.com/Gusb3ll/Euler-bot",
                },
                {
                    id: 6,
                    name: "gusbell-port",
                    sub: "Author",
                    desc: "This portfolio that are written in Nuxt.js",
                    to: "https://github.com/Gusb3ll/gusbell-port",
                    to2: "https://gusbell-port.vercel.app",
                },
            ],
        };
    },
};
</script>
