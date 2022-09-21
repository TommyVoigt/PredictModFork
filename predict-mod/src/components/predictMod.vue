<template>
    <div class="home">
      <Luisa :design="figmaConfig" v-model="viewModel" :config="config"/>
    </div>
  </template>
  
  <script>
  import Vue from "vue";
  import Figma from "vue-low-code";
  Vue.use(Figma);
  
  export default {
    name: "Home",
    data: function () {
      return {
        figmaConfig: {
          figmaFile: "o6jXvorQah0FxtmIzvxnx4",
          figmaAccessKey: "figd_dTYuXHVnZmXq-RPy5Fc_3lApgc5MH2IIAEpZ8dqK",
        },
        viewModel: {
          /**
           * Add your view model here
           */
        },
        config: {
          /**
           * Configure the reponsive behavior here. The 'page'
           * property is the name of the Figma page.
           **/
          responsive: [
            { page: "A", types: ["desktop"] },
            { page: "B", types: ["tablet", "mobile"] },
          ],
          components: {
            /**
             * Register costum components here
             */
          },
        },
      };
    },
    components: {},
    methods: {
      /**
       * Place your methods here
       */
    },
  };
  </script>