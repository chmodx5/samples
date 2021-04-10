<template>
    <div class="my-6">
        <v-container>
            <v-row>
                <v-col v-for="service in services" :key="service.id" class="text-center">
                    <v-card class="pa-3">
                        <div class="d-flex justify-center mb-3">
                            <span>
                                <v-img src="../assets/WarthogHead.svg" :aspect-ratio="1/1" width="100">
                                </v-img>
                            </span>
                        </div>
                        <h3 class="text-capitalize font-weight-bold text-h6"> {{service.title}} </h3>
                        <p> {{service.desc}} </p>
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
            services:[
                {
                    title: 'thing one',
                    desc: 'this is just some random short text to act as a placeholder text but looking at it irt seems to be too short for now, just a few more words  to meet the quota',
                    image: '../assets/WarthogHead.svg'
                },
                {
                    title: 'thing two',
                    desc: 'this is just some random short text to act as a placeholder text but looking at it irt seems to be too short for now, just a few more words  to meet the quota',
                    image: '../assets/WarthogHead.svg'
                },
                {
                    title: 'thing three',
                    desc: 'this is just some random short text to act as a placeholder text but looking at it irt seems to be too short for now, just a few more words  to meet the quota',
                    image: '../assets/WarthogHead.svg'
                },
            ]
        }
    }
}
</script>