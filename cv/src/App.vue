<template>
  <v-app>
    <v-main itemscope itemtype="http://schema.org/Person">
      <v-container>
        <header>
          <h1 itemprop="name"><span itemprop="givenName">Angelina</span> <span itemprop="familyName">Aïtkaci-Ali</span></h1>
          <h2>Développeuse Front-end</h2>
        </header>

        <Objectives/>
        <div class="content d-sm-flex">
          <Experience/>

          <section class="additionnal">

            <Skills/>
            <Training/>

            <Contact/>
          </section>

        </div>
      </v-container>

      <v-bottom-navigation
          v-if="isMobile()"
         scroll-threshold
          background-color="#3DD2CC"
          color="white"
          flat
          dense
          hide-on-scroll
          fixed
      >

        <v-btn>
          <a itemprop="telephone" href="tel:+33631789238"><v-icon>mdi-phone</v-icon></a>
        </v-btn>

        <v-btn>
          <a itemprop="url" rel="me" href="https://www.linkedin.com/in/aaitkaci" target="_blank" ><v-icon>mdi-linkedin</v-icon></a>
        </v-btn>

        <v-btn>
          <a itemprop="email" href="mailto:angelina.aitkaci@gmail.com" target="_blank"><v-icon>mdi-email</v-icon></a>
        </v-btn>

        <v-btn>
          <a href="../public/assets/Aitkaci-ali_Angelina.pdf" download="Aitkaci-ali_Angelina.pdf" target="_blank"><v-icon>mdi-content-save-outline</v-icon></a>
        </v-btn>

      </v-bottom-navigation>
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

    data () {
      return {
        publicPath: process.env.BASE_URL,
      }
    },

    methods: {
      isMobile() {
        if(/Android|webOS|iPhone|iPad|iPod|BlackBerry|IEMobile|Opera Mini/i.test(navigator.userAgent)) {
          return true
        } else {
          return false
        }
      },
    }
  });
</script>

<style lang="scss">

  @import '~vuetify/src/styles/styles.sass';
  $primary-color : #3DD2CC;
  $text-color: #3E6B89;

  ::-moz-selection { /* Code for Firefox */
    color: white;
    background: $primary-color;
  }
  ::selection {
    color: white;
    background: $primary-color;
  }
  body {
    border-bottom: 10px solid $primary-color;
  }
  main {
    margin: 0 15px 15px;
  }
  h1, h3, .theme--light.v-card .v-card__subtitle.subtitle {
    color: $primary-color;
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
    border-bottom: 3px solid $primary-color;
  }
  article {
    margin-bottom: 15px;
  }
  h3 {
    letter-spacing: 3px;
  }
  .theme--light.v-application {
    h2, .title, p, li {
      color: $text-color;
    }
  }

  /* mobile */
  @media #{map-get($display-breakpoints, 'sm-and-down')} {
    .v-application--is-ltr .v-timeline--dense:not(.v-timeline--reverse):before {
      left: calc(25px - 1px);
    }
    .v-timeline-item__divider {
      min-width: 50px;
    }
    .v-timeline--dense .v-timeline-item__body {
      max-width: calc(100% - 50px);
    }

  }

  @media #{map-get($display-breakpoints, 'md-and-down')} {

    .v-btn > .v-btn__content a {
      text-decoration: none;

      .v-icon {
        color: white;
      }
    }
  }
    /* laptop + desktop */
    @media #{map-get($display-breakpoints, 'md-and-up')} {
      /* style USELESS https://vuetifyjs.com/en/styles/flex/#enabling-flexbox */
    .content {
      display: -webkit-box;
      display: -moz-box;
      display: -ms-flexbox;
      display: -webkit-flex;
      display: flex;
      flex-direction: row;
      -ms-flex-direction: row;
      -webkit-flex-direction: row;
      align-items: stretch;
    }
    .additionnal {
      flex-basis: 35%;
      -webkit-flex-basis: 35%;
      order: 10;
      display: -webkit-box;
      display: -moz-box;
      display: -ms-flexbox;
      display: -webkit-flex;
      display: flex;
      flex-direction: column;
      -ms-flex-direction: column;
      -webkit-flex-direction: column;
      .contact {
        order:10;
      }
      .training {
        order:20;
      }
      .skills {
        order: 30;
      }
    }
    .experience {
      flex-basis: 65%;
      -webkit-flex-basis: 65%;
      order: 20;
    }

  }

</style>
