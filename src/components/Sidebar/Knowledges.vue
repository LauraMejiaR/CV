<template>
    <v-container class="text-center text-md-left">
        <div class="title text-center text-md-left mb-3">{{$t('sidebar.knowledges.title')}}</div>
        <v-list>
            <v-list-item-group>
                <v-list-item
                    v-for="(item, key, index) in $t('sidebar.knowledges.elements')" :key="index">
                    <v-list-item-title>{{item}}</v-list-item-title>
                </v-list-item>
            </v-list-item-group>
        </v-list>
    </v-container>
</template>

<script>
export default {
    name:'Knowledges',
}
</script>
