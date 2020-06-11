<template>
  <v-app>
    <v-app-bar
      app
      color="indigo darken-2"
      dark
      dense
    >
      <div class="d-flex align-center mr-4">
        <!-- <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-logo-dark.png"
          transition="scale-transition"
          width="40"
        /> -->

        <span class="display-1">
          MYTODO
        </span>
      </div>

      <v-btn
        link
        v-bind:to="'/'"
        text
      >
        <span class="mr-2">Home</span>
      </v-btn>
      
      <v-btn
        link
        v-bind:to="'about'"
        text
      >
        <span class="mr-2">About</span>
      </v-btn>
      

      <v-spacer></v-spacer>
    </v-app-bar>

    <v-content>
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
