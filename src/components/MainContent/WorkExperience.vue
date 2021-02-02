<template>
    <div>
        <div class="title text-center text-md-left">{{ $t('mainContent.workExperience.title')}}</div>
        <v-timeline dense class="mt-1">
            <v-timeline-item 
                fill-dot 
                color="secondary" 
                large
                v-for="(item, key, index) in $t('mainContent.workExperience.elements')"
                :key=(index)>
                <template v-slot:icon>
                    <v-avatar>
                        <img src="@/assets/Harman.png">
                    </v-avatar>
                </template>
                <v-card elevation="6">
                    <v-card-title class="pa-2">
                        {{item.workPlace}}<span class="text-caption">({{item.time}})</span>
                    </v-card-title>
                    <v-card-subtitle class="mt-0 text-button">{{item.position}}</v-card-subtitle>
                    <v-expansion-panels>
                        <v-expansion-panel>
                            <v-expansion-panel-header>
                                {{item.activities.title}}
                            </v-expansion-panel-header>
                            <v-expansion-panel-content>
                                <ul v-for="(activity,indexAct) in item.activities.elements" :key="indexAct" >
                                    <li>{{activity}}</li>
                                </ul>
                            </v-expansion-panel-content>
                        </v-expansion-panel>
                    </v-expansion-panels>
                </v-card>
            </v-timeline-item>
        </v-timeline>
    </div>
</template>

<script>
    export default {
        name: 'WorkExperience'
    }
</script>