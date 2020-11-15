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
      <header>
        <h1>Angelina Aïtkaci-Ali</h1>
        <h2>Développeuse Front-end</h2>
      </header>
      <Objectives/>

      <Experience/>gi

      <Skills/>

      <Training/>

      <Contact/>

    </v-main>
  </v-app>
</template>

<script>

  import Objectives from './components/Objectives';
  import Experience from './components/Experience';
  import Training from './components/Training';
  import Skills from './components/Skills';
  import Contact from './components/Contact';


  export default ({
    name: 'App',

    components: {
      Objectives,
      Experience,
      Training,
      Skills,
      Contact,
    },

    data: () => ({
      //
    }),
  });
</script>
