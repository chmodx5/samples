<template>
<div class="grey lighten-2">
    <v-container>
        <v-row class="hero-height">
            <v-col cols="12" md="5" class="d-flex align-center">
                <div>
                    <div>
                        <p class="text-h2 mb-0 text-capitalize font-weight-bold">providing</p>
                        <p class="secondary--text text-h2 mb-0 text-capitalize font-weight-bold"> fresh produce </p>
                        <p class="text-h2  text-capitalize font-weight-bold">everyday</p>
                    </div>
                    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Reprehenderit, autem! Excepturi, minus quia cum beatae nulla quos ducimus consequuntur at!</p>
                    <v-btn color="primary" rounded>learn more</v-btn>
                    <v-row class="mt-5">
                        <v-col v-for="my_itm in my_itms" :key="my_itm" class="">
                            <p class="font-weight-bold text-h6 text-capitalize"> {{my_itm.text}} <span>+</span></p>
                            <p class="text-subtitle-2">{{my_itm.total}}</p>
                        </v-col>
                    </v-row>
                </div>
            </v-col>
            <v-col cols="12" md="7" class="">
                <v-row justify="center" align="center" class="fill-height" >
                    <div>
                        <v-img src="../assets/WarthogHead.svg" :aspect-ratio="1/1" width="500">
                        </v-img>
                    </div>
                </v-row>
            </v-col>
        </v-row>
    </v-container>
</div>
</template>

<script>
  export default {
    name: 'heroSection',
    data(){
        return{
            my_itms:[
                {
                    total: '635',
                    text: 'subscribers'
                },
                {
                    total: '665',
                    text: 'followes'
                },
                {
                    total: '637465',
                    text: 'produce'
                },
            ]
        }
    },
    props:[],

  }
</script>
<style lang="scss" scoped>
.hero-height{
    height: 100vh;
}
</style>

