<template>
  <v-app>
    <v-app-bar
      app
      color="primary"
      dark
    >
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-logo-dark.png"
          transition="scale-transition"
          width="40"
        />

        <v-img
          alt="Vuetify Name"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="100"
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-name-dark.png"
          width="100"
        />
      </div>

      <v-spacer></v-spacer>

      <v-btn
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
        text
      >
        <span class="mr-2">Latest Release</span>
        <v-icon>mdi-open-in-new</v-icon>
      </v-btn>
    </v-app-bar>

    <v-main>
      <h1>Angelina Aïtkaci-Ali</h1>
      <h2>Développeuse Front-end</h2>
      <hr>
      <div>
        <h3>Coordonnées</h3>
        <p>
          <span class="material-icons">phone</span>
          <span>06 31 78 92 38</span>
        </p>
        <p>
          <span class="material-icons">email</span>
          <span>06 31 78 92 38</span>
        </p>
        <p>
          <span class="material-icons">location_searching</span>
          <span>06 31 78 92 38</span>
        </p>
        <p>
          <span class="material-icons">directions_car</span>
          <span>06 31 78 92 38</span>
        </p>
      </div>
      <div>
        <h3>Formation</h3>
        <v-timeline
            dense
            clipped
        >
          <v-timeline-item
              fill-dot
              small
              class="white--text mb-12"
              color="#3DD2CC"
              large
          >
            <v-card
                light
            >
              <v-card-title class="title">
                Formation Magento 2
              </v-card-title>
              <v-card-subtitle>
                Aout 2017 - Sept 2017
              </v-card-subtitle>
              <v-card-text class="white text--primary">
                <p>Clever Age</p>
              </v-card-text>
            </v-card>
          </v-timeline-item>
        </v-timeline>
      </div>
    </v-main>
  </v-app>
</template>

<script>

import Vue from 'vue';
import Vuetify from 'vuetify/lib';
import colors from 'vuetify/lib/util/colors'
import '@mdi/font/css/materialdesignicons.css';

Vue.use(Vuetify)

export default new Vuetify({
  name: 'App',
  theme: {
    themes: {
      light: {
        primary: colors.cyan.lighten-2, // #E53935
        secondary: colors.blueGrey.darken-4, // #37474F
        accent: colors.cyan.lighten-2, // #3F51B5
      },
    },
  },

  icons: {
    iconfont: 'mdi',
  },

  components: {
  },

  data: () => ({
    //
  }),
});
</script>
