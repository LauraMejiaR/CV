<template>
    <v-speed-dial 
        right
        fixed 
        bottom 
        fab
        direction="top"
        transition="slide-y-reverse-transition">
        <template v-slot:activator>
            <v-btn fab color="secondary" dark>
                <v-icon>fas fa-language</v-icon> <small class="ml-1">{{$i18n.locale}}</small>
            </v-btn>
        </template>
        <v-btn fab 
            dark 
            small 
            color="green" 
            @click="changeLanguage('es')"
            v-if="$i18n.locale !== 'es'">ES</v-btn>
        <v-btn fab 
            dark 
            small 
            color="indigo" 
            @click="changeLanguage('en')"
            v-if="$i18n.locale !== 'en'">EN</v-btn>
    </v-speed-dial>
</template>

<script>
    export default {
        name: 'ButtonLanguage',
        data(){
            return{
                langs: ['en','es']
            }
        },
        created(){
           this.$i18n.locale = 'es';
        },
        methods:{
            changeLanguage(lang){
                if (this.$i18n.locale !== lang) {
                    this.$i18n.locale = lang;
                }
            }
        }
    }
</script>