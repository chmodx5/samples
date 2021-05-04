<template>
    <v-container class="mod-hero">
        <v-row class="fill-height text-center" align="center" justify="center">
            <v-col lg="8">
                <p class="text-uppercase text-h5 primary--text my-3">
                    {{ coloredHeading }}
                </p>
                <p class="text-capitalize text-h3 styled-heading my-3 text-bold">
                     {{ heading }} 
                </p>
               
                <p class="text-h5 my-6">
                    {{ text }}
                </p>
                <v-btn :to="btnLink" color="primary" large>
                    {{ btnText }}
                </v-btn>
                <!-- <v-btn color="primary" @click="$vuetify.theme.dark =! $vuetify.theme.dark ">lnd</v-btn> -->
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
export default {
    name: 'modHero',
    data(){
        return{
        }
    },
    props: {
        coloredHeading: String,
        heading: String,
        text: String,
        btnText: String,
        btnLink: String
    }
}
</script>

<style lang="scss" scoped>
.mod-hero{
    height: 90vh;
    .styled-heading{
        display: inline-block;
        border: solid 3px ;
        border-left: none;
        border-right: none;
        // padding-top: 0.2em;
        // padding-bottom: .2em;
    }
}
</style>