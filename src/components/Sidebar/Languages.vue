<template>
    <v-container class="text-center text-md-left">
        <div class="title text-center text-md-left mb-3">{{$t('sidebar.languages.title')}}</div>
        <div v-for="(item,index) in $t('sidebar.languages.elements')" :key="index" class="mt-2">
            <p class="text-button mb-0">{{item.name}}</p>
            <v-progress-linear
                class="white--text"
                color="secondary" 
                :value="item.percent"
                height="25">
                {{item.percent}}%
             </v-progress-linear>
        </div>
    </v-container>
</template>

<script>
export default {
    name: 'Languages'
}
</script>