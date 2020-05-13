<template>
  <v-app>
    
    <v-bottom-navigation app dark>
      <v-spacer></v-spacer>
       <v-layout align-center>
        <v-btn to="/">
          <v-icon>mdi-home</v-icon>
        </v-btn>
        <v-btn to="/events">
          <v-icon>mdi-calendar</v-icon>
        </v-btn>
        <v-btn to="/about">
          <v-icon>mdi-account</v-icon>
        </v-btn>
       </v-layout>
    </v-bottom-navigation>
 
    <v-content>
      <v-container>
        <router-view></router-view>
      </v-container>
    </v-content>

  </v-app>
</template>

<script>
export default {
  name: 'App',

  components: {

  },

  data: () => ({
    //
  }),
};
</script>
