<template>
<v-card outlined class="mx-16 py-4" style="background-color: rgba(0, 0, 0, 0.3);">
    <v-row 
        v-for="skill in skills"
        :key="skill.id"
        justify="center">
        <v-col cols="12">
            <p class="text-h7 text-center text-sm-h6">{{ skill.title }}</p>
        </v-col>
        <v-col class="mt-n6" cols="8">
            <v-progress-linear :color="skill.color" rounded class="mb-4" height="8" :value="skill.value"></v-progress-linear>
        </v-col>
    </v-row>
</v-card>
</template>

<script lang="ts">
export default {
    name: 'langSkill',
    data() {
        return {
            skills: [
                {
                    id: 1,
                    title: 'HTML',
                    color: 'cyan darken-2',
                    value: '100'
                },
                {
                    id: 2,
                    title: 'CSS',
                    color: 'cyan darken-2',
                    value: '95'
                },
                {
                    id:3,
                    title: 'JavaScript',
                    color: 'yellow darken-2',
                    value: '75'
                },
                {
                    id:4,
                    title: 'Vue',
                    color: 'green darken-2',
                    value: '85'
                },
                {
                    id:5,
                    title: 'Python',
                    color: 'yellow darken-2',
                    value: '85'
                },
                {
                    id:6,
                    title: 'Frontend',
                    color: 'purple lighten-2',
                    value: '82'
                },
                {
                    id:7,
                    title: 'Backend',
                    color: 'purple lighten-2',
                    value: '52'
                }
            ]
        }
    }
}
</script>
