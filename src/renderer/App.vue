<template>
  <v-app dark>
    <v-toolbar fixed app>
      <v-spacer class="hidden-sm-and-down"></v-spacer>
      <v-toolbar-title class="hidden-sm-and-down" v-text="title"></v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn>
        <v-icon>invert_colors</v-icon>
      </v-btn>
      <v-btn>
        <v-icon>settings</v-icon>
      </v-btn>
    </v-toolbar>

    <v-content>
      <v-container fluid fill-height>
        <v-layout row wrap justify-center id="wrapper">
          <v-flex xs10 class="mt-3">
            <v-card>
              <v-card-text>
                <p>Hello World.</p>
              </v-card-text>
            </v-card>
          </v-flex>
        </v-layout>
      </v-container>
    </v-content>

    <v-footer app>
      <v-spacer></v-spacer>
      <span>&copy; 2018</span>
    </v-footer>
    <!--
    -->
  </v-app>
</template>

<script>
  export default {
    name: 'electify',
    data: () => ({
      title: 'Vuetify.js'
    })
  }
</script>

<style>
  @import url('https://fonts.googleapis.com/css?family=Roboto:300,400,500,700|Material+Icons');
  /* Global CSS */
</style>
