<template>
  <v-app>
    <v-main>
      <v-scroll-x-transition appear>
        <v-container>
          <Header />
          <Content />
        </v-container>
      </v-scroll-x-transition>
      <ButtonLanguage />
    </v-main>
    <v-footer app absolute padless>
      <v-col class="text-center" cols="12">
        <div class='caption'>Created by <a color="secondary" href="https://www.linkedin.com/in/julio-cesar-vazquez-c/">Julio Cesar Vazquez Cervantes</a></div>
      </v-col>
    </v-footer>
  </v-app>
</template>

<script>
  import Header from './components/Header';
  import Content from './components/Content';
  import ButtonLanguage from './components/ButtonLanguage';

  export default {
    name: 'App',

    components: {
      Header,
      Content,
      ButtonLanguage
    },

    data: () => ({
      change: false
    }),
  };
</script>