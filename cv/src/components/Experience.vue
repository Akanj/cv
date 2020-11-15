<template>

  <section>
    <h3>Expériences</h3>
    <v-timeline
        clipped
        dense
    >
      <v-timeline-item
          fill-dot
          small
          class="white--text mb-12"
          color="#3DD2CC"
          itemprop="worksFor"
          itemscope
          itemtype="http://schema.org/Organization"
      >
        <v-card>
          <v-card-title class="title">
            <span itemprop="jobTitle">Lead Technique Magento 2</span> - <span itemprop="name">API & YOU</span>
          </v-card-title>
          <v-card-text class="white text--primary">
            <v-card-subtitle class="subtitle">
              FÉV 2019 - AUJOURD'HUI
            </v-card-subtitle>
            <ul itemprop="description">
              <li>Compréhension des attentes et problématiques du client</li>
              <li>Participation à l'élaboration du cahier des charges fonctionnel</li>
              <li>Estimation des temps de développement</li>
              <li>Gestion du planning (4 pers.)</li>
              <li>Formation des équipes (front et admin)</li>
              <li>Rédaction de documentation</li>
              <li>Rédaction des procédures</li>
              <li>Contrôle qualité des livraisons</li>
              <li>Développement/Debug de modules PHP</li>
            </ul>
          </v-card-text>
        </v-card>
      </v-timeline-item>

      <v-timeline-item
          fill-dot
          small
          class="white--text mb-12"
          color="#3DD2CC"
          itemscope
          itemtype="http://schema.org/Event/Job"
      >
        <v-card>
          <v-card-title class="title">
            <span itemprop="name">Développeuse Front-end</span> - API & YOU
          </v-card-title>
          <v-card-subtitle class="subtitle">
            <span itemprop="startDate" content="2017-01-21T20:00">JAN 2017</span> - <span itemprop="endDate" content="2019-02-21T20:00">FÉV 2019</span>
          </v-card-subtitle>
          <v-card-text class="white text--primary">
            <ul itemprop="description">
              <li>Développement front-end Magento 2</li>
              <li>Analyse et résolution des dysfonctionnements</li>
              <li>Mise en place et respect de process pour la structure des projets</li>
              <li>Gestion des mises en production</li>
              <li>Maintenance des livrables en production</li>
              <li>Dynamique type start-up ( 6 pers.)</li>
            </ul>
          </v-card-text>
        </v-card>
      </v-timeline-item>

      <v-timeline-item
          fill-dot
          small
          class="white--text mb-12"
          color="#3DD2CC"
          itemscope
          itemtype="http://schema.org/Event/Job"
      >
        <v-card>
          <v-card-title class="title">
            <span itemprop="name">Intégratrice Web</span> - API & YOU
          </v-card-title>
          <v-card-subtitle class="subtitle">
            <span itemprop="startDate" content="2015-05-21T20:00">MAI 2015</span> - <span itemprop="endDate" content="2017-01-21T20:00">JAN 2017</span>
          </v-card-subtitle>
          <v-card-text class="white text--primary">
            <ul itemprop="description">
              <li>Création de sites vitrines utilisant un CMS propriétaire basé Symfony 2.8marketing</li>
              <li>Participation aux mêlées quotidiennesmarketing</li>
              <li>Recherche de solutions techniques à des problèmes marketing</li>
            </ul>
          </v-card-text>
        </v-card>
      </v-timeline-item>

    </v-timeline>
  </section>

</template>

<script>
  export default {
    name: 'Experience',

    data: () => ({
      ecosystem: [
        {
          text: 'vuetify-loader',
          href: 'https://github.com/vuetifyjs/vuetify-loader',
        },
        {
          text: 'github',
          href: 'https://github.com/vuetifyjs/vuetify',
        },
        {
          text: 'awesome-vuetify',
          href: 'https://github.com/vuetifyjs/awesome-vuetify',
        },
      ],
      importantLinks: [
        {
          text: 'Documentation',
          href: 'https://vuetifyjs.com',
        },
        {
          text: 'Chat',
          href: 'https://community.vuetifyjs.com',
        },
        {
          text: 'Made with Vuetify',
          href: 'https://madewithvuejs.com/vuetify',
        },
        {
          text: 'Twitter',
          href: 'https://twitter.com/vuetifyjs',
        },
        {
          text: 'Articles',
          href: 'https://medium.com/vuetify',
        },
      ],
      whatsNext: [
        {
          text: 'Explore components',
          href: 'https://vuetifyjs.com/components/api-explorer',
        },
        {
          text: 'Select a layout',
          href: 'https://vuetifyjs.com/getting-started/pre-made-layouts',
        },
        {
          text: 'Frequently Asked Questions',
          href: 'https://vuetifyjs.com/getting-started/frequently-asked-questions',
        },
      ],
    }),
  }
</script>
