<template>

  <article class="contact" :class="className">
    <h3>Coordonnées</h3>
    <p>
      <v-icon>mdi-phone</v-icon>
      <a itemprop="telephone" href="tel:+33631789238">06 31 78 92 38</a>
    </p>
    <p>
      <v-icon>mdi-email</v-icon>
      <a itemprop="email" href="mailto:angelina.aitkaci@gmail.com">angelina.aitkaci@gmail.com</a>
    </p>
    <p>
      <v-icon>mdi-target</v-icon>
      <span itemprop="homeLocation">Jura</span> - Mobile en France</p>
    <p>
      <v-icon>mdi-car</v-icon>

      <span>Permis B - Vehicule</span>
    </p>
    <p>
      <a itemprop="url" rel="me" href="https://www.linkedin.com/in/aaitkaci">https://www.linkedin.com/in/aaitkaci</a>
    </p>
  </article>
</template>

<script>
import Vue from 'vue'
import Vuetify from 'vuetify/lib'

Vue.use(Vuetify)

export default new Vuetify({
  name: "Contact",
  icons: {
    iconfont: 'mdi',
  },
  props: ['className']

});



</script>

<style lang="scss" scoped>
  .mdi {
    margin-right: 15px;
    color: #3DD2CC;
  }

  .theme--light.v-application a {
      color: #3E6B89;
  }

</style>
