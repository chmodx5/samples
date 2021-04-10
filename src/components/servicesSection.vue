<template>
    <div class="my-6">
        <v-container>
            <v-row>
                <v-col v-for="i in 3" :key="i" class="text-center">
                    <v-card class="pa-3">
                        <div class="d-flex justify-center mb-3">
                            <span>
                                <v-img src="../assets/WarthogHead.svg" :aspect-ratio="1/1" width="100">
                                </v-img>
                            </span>
                        </div>
                        <h3>thing one</h3>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestias alias cumque atque nisi odit fuga!</p>
                    </v-card>
                </v-col>
            </v-row>
        </v-container>
    </div>
</template>

<script>
export default {
    name: 'servicesSection',
    data(){
        return{

        }
    }
}
</script>