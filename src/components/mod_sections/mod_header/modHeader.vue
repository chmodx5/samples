<template>
    <v-app-bar
      app
      height="50"
      color="white"
      elevate-on-scroll
    >
      <v-container class="py-0 fill-height">
        <h1 class="text-uppercase text-h5 font-weight-bold"><span class="primary--text">war</span>thog</h1>
        <v-spacer></v-spacer>
        <!-- this is looping through the list of all the routes in vue router -->
        <v-btn
          v-for="route in $router.options.routes"
          :key="route.path"
          :to="route.path"
          text
          plain
          active-class="mod-active"
        >
          {{ route.name }}
        </v-btn>
        <v-btn color="primary" flat depressed>
          sign up
        </v-btn>
      </v-container>
    </v-app-bar>
</template>

<script>
export default {
    name: 'modHeader',
    data(){
        return{

        }
    }
}
</script>

<style lang="scss" scoped>
// .mod-active{
//   // background-color: aqua;
//   // color: aqua !important;
// }
</style>