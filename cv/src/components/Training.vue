<template>
  <article class="training">
    <h3>Formation</h3>
    <v-timeline
        dense
        clipped
    >
      <v-timeline-item
          fill-dot
          small
          class="white--text mb-1"
          color="#3DD2CC"
          itemprop="alumniOf"
          itemscope
          itemtype="http://schema.org/EducationalOrganization">
        <v-card
            elevation="1"
            tile>
          <v-card-title class="title" itemprop="description">
            Formation Magento 2
          </v-card-title>
          <v-card-subtitle class="subtitle">
            Aout 2017 - Sept 2017
          </v-card-subtitle>
          <v-card-text class="white text--primary">
            <p itemprop="name">Clever Age</p>
          </v-card-text>
        </v-card>
      </v-timeline-item>
      <v-timeline-item
          fill-dot
          small
          class="white--text mb-1"
          color="#3DD2CC"
          itemprop="alumniOf"
          itemscope
          itemtype="http://schema.org/EducationalOrganization"
      >
        <v-card>
          <v-card-title class="title" itemprop="description">
            Formation Web Designer
          </v-card-title>
          <v-card-subtitle class="subtitle">
            SEPT 2013 - JUIN 2014
          </v-card-subtitle>
          <v-card-text class="white text--primary">
            <p><span itemprop="name">DGD Formation</span> - <span itemprop="location">Vesoul</span><br>Titre professionnel Niveau V</p>
          </v-card-text>
        </v-card>
      </v-timeline-item>
      <v-timeline-item
          fill-dot
          small
          class="white--text mb-1"
          color="#3DD2CC"
          itemprop="alumniOf"
          itemscope
          itemtype="http://schema.org/EducationalOrganization"
      >
        <v-card>
          <v-card-title class="title" itemprop="name">
            UFR Sciences et Techniques
          </v-card-title>
          <v-card-subtitle class="subtitle">
            SEPT 2011 - JUIL 2012
          </v-card-subtitle>
          <v-card-text class="white text--primary">
            <p itemprop="description">Licence en sciences physiques</p>
          </v-card-text>
        </v-card>
      </v-timeline-item>
    </v-timeline>
  </article>
</template>

<script>
export default {
  name: "Training"
}
</script>

<style scoped>

</style>
