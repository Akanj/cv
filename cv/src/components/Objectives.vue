<template>
  <article itemprop="description" class="objectives">
    <p>Lead Technique Magento 2 et forte de 5 ans d'expérience en agence de communication, je souhaite me tourner vers le développement JavaScript (ES6, TypeScript, Vue, React, Angular...).</p>
    <p>Comme mon parcours en témoigne, je sais faire preuve d'une grande agilité, de résilience et d'adaptabilité. Je cherche continuellement à monter en compétences par l'échange avec mon équipe et l'auto-formation.</p>
  </article>
</template>

<script>
export default {
name: "Objectives"
}
</script>

<style lang="scss" scoped>

@import '~vuetify/src/styles/styles.sass';

@media #{map-get($display-breakpoints, 'sm-and-up')} {
  .objectives {
    margin-bottom: 30px ;
  }
}
</style>
