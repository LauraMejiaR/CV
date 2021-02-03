<template>
   <v-card>
       <v-container class="background">
           <v-row>
                <v-col cols=12 md="4" align="center" class="mb-md-n16">
                    <v-img
                     id="profile"
                     class="elevation-6 rounded"
                     width="400px"
                     src="@/assets/Lau.jpeg">
                    </v-img>
                </v-col>
                <v-col cols=12 md="8" class="white--text text-center text-md-left" >
                    <p class='text-h4 not-margin'>{{$t('header.name')}}</p>
                    <p class='text-subtitle-1'>{{$t('header.degree')}}</p>
                    <p><v-icon small>fas fa-map-marker-alt</v-icon> {{$t('header.address')}} </p>
                    <p><v-icon small>fas fa-envelope</v-icon> {{$t('header.email')}} </p>
                    <p><v-icon small>fas fa-phone</v-icon> {{$t('header.phone')}} </p>
                    <p><v-icon small>fas fa-birthday-cake</v-icon> {{$t('header.years')}} </p>
                    <p>
                        <a href="https://www.linkedin.com/in/ana-laura-mejia-ramirez-5195a61a2/" target=_blank>
                            <v-icon color="white">fab fa-linkedin</v-icon>
                        </a>
                        Linkedin
                    </p>
                </v-col>
            </v-row>
       </v-container>
   </v-card>
</template>

<script>
export default {
    name: 'Header'
}
</script>

<style scoped>
    #profile{
        z-index: 1;
    }
    .not-margin{
        margin-bottom: 0px;       
    }
    .v-icon{
        color: white !important;
    }
    .background{
        background: rgb(205,213,241);
        background: linear-gradient(24deg, rgba(52, 52, 58, 0.906) 30%, rgb(20, 20, 20) 61%);
    }
</style>