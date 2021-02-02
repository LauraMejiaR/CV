<template>
    <v-container>
        <WorkExperience/>
        <Education/>
    </v-container>
</template>

<script>
    import WorkExperience from './MainContent/WorkExperience'
    import Education from './MainContent/Education'
    export default {
        name: 'MainContent',
        components:{
            WorkExperience,
            Education
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