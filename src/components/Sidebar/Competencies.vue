<template>
    <v-container>
        <div class="title text-center text-md-left">{{$t('sidebar.competencies.title')}}</div>
        <template>
            <v-row no-gutters class="text-center">
                <v-col v-for="(item,key, index) in $t('sidebar.competencies.elements')" :key="index" class="d-inline"
                    cols="6" md="4">
                    <v-progress-circular rotate="360" size="100" width="2" value="100" :color="colors[index]"
                        class="ma-2 text-center">
                        {{item}}
                    </v-progress-circular>
                </v-col>
            </v-row>
        </template>
    </v-container>
</template>

<script>
    export default {
        name: 'Competencies',
        data() {
            return {
                colors: ['accent', 'info', 'success', 'warning']
            }
        }
    }
</script>

