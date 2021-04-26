<template>
    <mod-section secHeading='what i do'>
        <v-row>
            <v-col md="4" v-for="service in myServices" :key="service.id">
                <v-card class="pa-12" hover max-height="350">
                    <v-sheet
                        outlined
                        height="70"
                        width="70"
                        elevation="1"
                        class="d-flex justify-center mb-6"
                    >
                        <v-icon color="primary" x-large>
                            {{ service.icon }}
                        </v-icon> 
                    </v-sheet>
                    <h3 class="text-h5 mb-3"> {{ service.heading }} </h3>
                    <v-sheet height="100" class="overflow-hidden" >
                        <p style="width:100%" class="mb-3 text-justify "> {{ service.desc }} </p>
                    </v-sheet>
                    
                    <v-btn text :to="service.link">read more</v-btn>
                </v-card>
            </v-col>
        </v-row>   
    </mod-section>
</template>

<script>
import modSection from '@/components/mod_sections/mod_slots/modSection.vue'

export default {
    name: 'modServicesSection',
    components: {
        modSection
    },
    data(){
        return{
             myServices: [
                 {
                     icon: 'mdi-earth',
                     heading: 'something somthing',
                     desc: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Delectus porro suscipit rerum commodi labore debitis nesciunt quibusdam est ipsum voluptatum?',
                     link: '/'
                 },
                 {
                     icon: 'mdi-earth',
                     heading: 'something somthing',
                     desc: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Delectus porro suscipit rerum commodi labore debitis nesciunt quibusdam est ipsum voluptatum?',
                     link: '/'
                 },
                 {
                     icon: 'mdi-earth',
                     heading: 'something somthing',
                     desc: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Delectus porro suscipit rerum commodi labore debitis nesciunt quibusdam est ipsum voluptatum?Lorem ipsum dolor, sit amet consectetur adipisicing elit. Delectus porro suscipit rerum commodi labore debitis nesciunt quibusdam est ipsum voluptatum?',
                     link: '/'
                 },
             ]
        }
    }
}
</script>

 <style lang="scss">
 .mod-card-icon{
     border: solid 1px black;
     background: blue;
     display: inline-block;

 }
 </style>