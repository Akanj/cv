<template>
  <v-app>
    <v-main itemscope itemtype="http://schema.org/Person">
      <header>
        <h1 itemprop="name"><span itemprop="givenName">Angelina</span> <span itemprop="familyName">Aïtkaci-Ali</span></h1>
        <h2>Développeuse Front-end</h2>
      </header>

      <Objectives/>

      <Experience/>

      <section>
        <Skills/>
        <Training/>
      </section>

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

<style lang="scss">
  * {
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
  }
  ::-moz-selection { /* Code for Firefox */
    color: white;
    background: #3DD2CC;
  }
  ::selection {
    color: white;
    background: #3DD2CC;
  }
  main {
    margin: 0 15px 15px;
  }
  h1, h3, .theme--light.v-card .v-card__subtitle.subtitle {
    color: #3DD2CC;
    text-transform: uppercase;
  }
  h1, h2 {
    text-transform: uppercase;
    text-align: center;
  }
  h1 {
    letter-spacing: 10px;
    margin-bottom: 20px;
  }
  h2 {
    letter-spacing: 6px;
    margin-bottom: 15px;
  }
  h3 {
    margin-bottom: 15px;
  }
  header {
    margin: 15px 0 30px;
    border-bottom: 3px solid #3DD2CC;
  }
  article {
    margin-bottom: 15px;
  }

  h3 {
    letter-spacing: 3px;
  }
  .theme--light.v-application {
    h2, .title, p, li, a {
      color: #3E6B89;
    }
  }
  .mdi {
    color: #3DD2CC;
  }

  @media screen and (max-width: 768px) {
    .v-application--is-ltr .v-timeline--dense:not(.v-timeline--reverse):before {
      left: calc(25px - 1px);
    }
    .v-timeline-item__divider {
      min-width: 50px;
    }
  }

</style>
