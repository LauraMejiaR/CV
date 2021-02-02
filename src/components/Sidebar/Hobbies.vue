<template>
    <v-container class="text-center text-md-left">
        <div class="title text-center text-md-left mb-3">{{$t('sidebar.hobbies.title')}}</div>
        <v-chip  v-for="(item,index) in $t('sidebar.hobbies.elements')" :key="index" class="mr-2 mt-2">
            <v-avatar>
                <v-icon small class="mr-1">
                    {{item.icon}}
                </v-icon>
            </v-avatar>
            {{item.title}}
        </v-chip>
    </v-container>
</template>

<script>
    export default {
        name: 'Hobbies'
    }
</script>