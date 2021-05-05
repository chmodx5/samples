<template>
    <mod-section secHeading='portfolio'>
        <v-card>
            <v-tabs
            color="primary "
            >
                <v-tab 
                    v-for="category in categories" 
                    :key=" category.id"
                >
                    {{ category }}    
                </v-tab>
                

                <v-tab-item
                    v-for="categoryItem in categoryItems"
                    :key="categoryItem"
                >
                    <v-container fluid>
                    <v-row>
                        <v-col
                        v-for="i in 6"
                        :key="i"
                        cols="12"
                        md="4"
                        >
                        <v-img
                            :src="`https://picsum.photos/500/300?image=${i * i * 5 + 10}`"
                            :lazy-src="`https://picsum.photos/10/6?image=${i * i * 5 + 10}`"
                            aspect-ratio="1"
                        ></v-img>
                        </v-col>
                    </v-row>
                    </v-container>
                </v-tab-item>
            </v-tabs>
        </v-card>
    </mod-section>
</template>

<script>
import modSection from '@/components/mod_sections/mod_slots/modSection.vue'

export default {
    name: 'modPortfolioSection',
    components: {
        modSection
    },
    data(){
        return{
            
        }
    },
    props: {
        categories: Array,
        categoryItems: Array
    }
}
</script>
