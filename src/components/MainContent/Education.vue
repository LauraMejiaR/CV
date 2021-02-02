<template>
    <div class='mt-1'>
        <div class="title text-center text-md-left">{{ $t('mainContent.education.title')}}</div>
        <v-timeline align-top dense class="mt-1">
            <v-timeline-item color="info" 
                v-for="(item, key, index) in $t('mainContent.education.elements')"
                :key=(index)>
                <v-row class="pt-1">
                    <v-col cols="3">
                        <strong class="caption">{{item.period}}</strong>
                    </v-col>
                    <v-col>
                        <strong>{{item.career}}</strong>
                        <div class="caption">{{item.school}}</div>
                    </v-col>
                </v-row>
            </v-timeline-item>
        </v-timeline>
    </div>
</template>

<script>
    export default {
        name: 'Education'
    }
</script>