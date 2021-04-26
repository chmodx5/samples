<template>
  <div>
    <mod-hero></mod-hero>
    <mod-about-section></mod-about-section>
    <mod-services-section></mod-services-section>
    <mod-portfolio-section></mod-portfolio-section>
    <mod-contact-section></mod-contact-section>
  </div>
</template>

<script>

import modHero from '@/components/mod_sections/mod_hero/modHero.vue'
import modAboutSection from '@/components/mod_sections/mod_main/modAboutSection.vue'
import modServicesSection from '@/components/mod_sections/mod_main/modServicesSection.vue'
import modPortfolioSection from '@/components/mod_sections/mod_main/modPortfolioSection.vue'
import modContactSection from '@/components/mod_sections/mod_main/modContactSection.vue'
//import modHeroOne from '@/components/mod_sections/mod_hero/modHeroOne.vue'

export default {
  name: 'Home',
  components: {
    modHero,
    modAboutSection,
    modServicesSection,
    modPortfolioSection,
    modContactSection
  }
}
</script>

<style lang="scss" scoped>
   

</style>