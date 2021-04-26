<template>
    <v-container class="mod-hero">
        <v-row class="fill-height text-center" align="center" justify="center">
            <v-col lg="8">
                <p class="text-uppercase text-h5 primary--text my-3">visual designer</p>
                <p class="text-capitalize text-h3 styled-heading my-3">i'm someone else</p>
               
                <p class="text-subtitle-1 my-6">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Accusantium similique quo laboriosam eius. Optio, commodi. Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatum incidunt, sit optio cumque perferendis accusantium.</p>
                <v-btn color="primary" large>
                    donwload cvs
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