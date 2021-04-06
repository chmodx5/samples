<template>
  <div>
    <hero-section></hero-section>
  </div>
</template>

<script>
// @ is an alias to /src
import heroSection from '@/components/heroSection.vue'

export default {
  name: 'Home',
  components: {
    heroSection
  }
}
</script>

<style lang="scss" scoped>

</style>