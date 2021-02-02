<template>
    <v-container class="pa-0">
        <Competencies />
        <Hobbies/>
        <Languages/>
        <Knowledges/>
    </v-container>
</template>

<script>
    import Competencies from './Sidebar/Competencies';
    import Hobbies from './Sidebar/Hobbies';
    import Languages from './Sidebar/Languages';
    import Knowledges from './Sidebar/Knowledges';
    export default {
        name: 'Sidebar',
        components: {
            Competencies,
            Hobbies,
            Languages,
            Knowledges
        }
    }
</script>

<style scoped>
    /deep/ .title {
        border-bottom: 2px #bfbfbf solid;
        font-weight: 300;
        line-height: 1.5 !important;
        letter-spacing: 0.2em !important;
    }
</style>