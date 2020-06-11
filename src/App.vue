<template>
  <v-app class="blue-grey lighten-4">
    <v-app-bar
      app
      color="blue-grey lighten-4"
      elevate-on-scroll  >

  <v-toolbar-title>
    MYTODO
  </v-toolbar-title>
      <v-btn
        link
        v-bind:to="'/'"
        text
        class="ml-4"
      >
        <span class="mr-2">Home</span>
      </v-btn>
      
      <v-btn
        link
        v-bind:to="'cca'"
        text
        class="ml-2"
      >
        <span class="mr-2">CCA</span>
      </v-btn>
      <v-btn
        link
        v-bind:to="'about'"
        text
        class="ml-2"
      >
        <span class="mr-2">About</span>
      </v-btn>

      <v-spacer></v-spacer>
    </v-app-bar>

    <v-content class="blue-grey lighten-4">
      <!-- Provides the application the proper gutter -->
      <v-container fluid>
        <!-- If using vue-router -->
        <router-view></router-view>
      </v-container>    
    </v-content>
  </v-app>
</template>

<script>
// import HelloWorld from './components/HelloWorld';

export default {
  name: 'App',

  components: {
    // HelloWorld,
  },

  data: () => ({
    //
  }),
};
</script>
