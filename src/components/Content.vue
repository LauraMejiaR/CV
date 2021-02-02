<template>
    <v-container class='mt-6'>
        <v-row>
            <v-col cols="12" md="4">
                <v-card elevation="3">
                    <Sidebar/>
                </v-card>
            </v-col>
            <v-col cols="12" md="8">
                <MainContent/>
            </v-col>
        </v-row>
        
    </v-container>
</template>

<script>
import Sidebar from './Sidebar';
import MainContent from './MainContent'
export default {
    name: 'Content',
    components:{
        Sidebar,
        MainContent
    }
}
</script>