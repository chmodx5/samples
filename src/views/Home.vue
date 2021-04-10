<template>
  <div>
    <hero-section></hero-section>
    <small-banner-section></small-banner-section>
    <services-section></services-section>
  </div>
</template>

<script>
// @ is an alias to /src
import heroSection from '@/components/heroSection.vue'
import smallBannerSection from '@/components/smallBannerSection.vue'
import servicesSection from '@/components/servicesSection.vue'

export default {
  name: 'Home',
  components: {
    heroSection,
    smallBannerSection,
    servicesSection
  }
}
</script>

<style lang="scss" scoped>

</style>