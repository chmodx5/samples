<template>
  <div>
    <mod-hero></mod-hero>
    <mod-hero-one></mod-hero-one>
  </div>
</template>

<script>

import modHero from '@/components/mod_sections/mod_hero/modHero.vue'
import modHeroOne from '@/components/mod_sections/mod_hero/modHeroOne.vue'

export default {
  name: 'Home',
  components: {
    modHero,
    modHeroOne
  }
}
</script>

<style lang="scss" scoped>
   

</style>