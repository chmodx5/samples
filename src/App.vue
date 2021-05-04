<template>
  <v-app id="inspire" >
    
    <mod-header></mod-header>

    <v-main class="lighten-3">
      <router-view></router-view>
    </v-main>

    <mod-footer></mod-footer>
  </v-app>
</template>
 
<script>
import modHeader from '@/components/mod_sections/mod_header/modHeader.vue';
import modFooter from '@/components/mod_sections/mod_footer/modFooter.vue'
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
      modHeader,
      modFooter
    }
  }
</script>

<style lang="scss">

</style>