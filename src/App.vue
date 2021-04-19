<template>
  <v-app id="inspire">
    <mod-header></mod-header>

    <v-main class="lighten-3">
      <router-view></router-view>
    </v-main>
  </v-app>
</template>
 
<script>
import modHeader from '@/components/mod_sections/mod_header/modHeader.vue'
  export default {
    data: () => ({
      links: [
        'Dashboard',
        'Messages',
        'Profile',
        'Updates',
      ],
    }),
    components: {
      modHeader
    }
  }
</script>

<style lang="scss">

</style>