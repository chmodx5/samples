<template>
  <v-app id="inspire">
    <v-app-bar
      app
      color="white"
      flat
    >
      <v-container class="py-0 fill-height">
        <h1 class="text-uppercase text-h5 font-weight-bold"><span class="secondary--text">war</span>thog</h1>
        <v-spacer></v-spacer>
        <!-- this is looping through the list of all the routes in vue router -->
        <v-btn
          v-for="route in $router.options.routes"
          :key="route.path"
          :to="route.path"
          text
        >
          {{ route.name }}
        </v-btn>

        <v-spacer></v-spacer>
        <v-btn color="primary" rounded>
          sign up
        </v-btn>
      </v-container>
    </v-app-bar>

    <v-main class="lighten-3">
      <router-view></router-view>
    </v-main>
  </v-app>
</template>
 
<script>
  export default {
    data: () => ({
      links: [
        'Dashboard',
        'Messages',
        'Profile',
        'Updates',
      ],
    }),
  }
</script>

<style lang="scss">

</style>