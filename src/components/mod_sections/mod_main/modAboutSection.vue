<template>
    <mod-section :secHeading='sectionHeading'>
        <v-row>
            <v-col cols="12" md="4">
                <v-img
                    :aspect-ratio="9/9"
                    :lazy-src="lazyImg"
                    :src="img"
                    :alt="imgAlt"
                    height="100%"
                ></v-img>
            </v-col>
            <v-col md="8" class="px-6"> 
                <v-simple-table>
                    <template v-slot:default>
                        <tbody>
                            <tr
                            v-for="item in info"
                            :key="item.id"
                            >
                            <td>
                                <v-icon
                                medium
                                color="primary"
                                class="mr-3"
                                >
                                {{ item.icon }}
                                </v-icon>
                                {{ item.title }} 
                            </td>
                            <td>
                                <span class="mr-3">:</span>
                                {{ item.info }}
                            </td>
                            </tr>
                        </tbody>
                    </template>
                </v-simple-table>
                <div class="mt-6">
                    <h1 class="text-h5 text-capitalize mb-3">
                        {{ heading }}
                    </h1>
                    <p class="mb-6">
                        {{ text }}
                    </p>
                    <v-btn :to="btnLink" color="primary"> {{ btnText }} </v-btn>
                </div>
            </v-col>
        </v-row>
    </mod-section>
</template>

<script>
//import modSecHeading from '@/components/mod_single_comps/mod_text/modSecHeading.vue'
import modSection from '@/components/mod_sections/mod_slots/modSection.vue'

export default {
    name: 'modAboutSection',
    components: {
        //modSecHeading,
        modSection
    },
    data(){
        return{
        }
    },
    props:{
        sectionHeading: String,
        img : String,
        lazyImg : String,
        imgAlt: String,
        info: Array,
        heading: String,
        text: String,
        btnText: String,
        btnLink: String,

    }
}
</script>

<style lang="scss">
// .about-section-heading{
//     text-decoration: underline;
// }
</style>