<template>
  <div id="app">
    <v-app dark>
      <v-toolbar dense fixed app color="primary">
        <v-spacer class="hidden-sm-and-down"></v-spacer>
        <v-toolbar-title class="hidden-sm-and-down" v-text="title"></v-toolbar-title>
        <v-spacer></v-spacer>
        <v-btn>
          <v-icon>fa-adjust</v-icon>
        </v-btn>
        <v-btn>
          <span class="hidden-xs-only">Update PLA List&nbsp;</span>
          <v-icon>fa-list</v-icon>
        </v-btn>
        <v-btn>
          <span class="hidden-xs-only">Settings&nbsp;</span>
          <v-icon>fa-cog</v-icon>
        </v-btn>
      </v-toolbar>
      <v-content>
        <v-container fluid fill-height>
          <welcome-view></welcome-view>
        </v-container>
      </v-content>
      <v-footer :fixed="fixed" app>
        <v-spacer></v-spacer>
        <span>&copy; 2017</span>
      </v-footer>
    </v-app>
  </div>
</template>

<script>
  import WelcomeView from '@/components/WelcomeView'
  export default {
    name: 'electify',
    components: {
      WelcomeView
    },
    data: () => ({
      clipped: false,
      drawer: true,
      fixed: false,
      items: [
        { icon: 'apps', title: 'Welcome', to: '/' },
        { icon: 'bubble_chart', title: 'Inspire', to: '/inspire' }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js'
    })
  }
</script>

<style>
  @import url('https://fonts.googleapis.com/css?family=Roboto:300,400,500,700|Material+Icons');
  /* Global CSS */
</style>
