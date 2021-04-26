<template>
    <mod-section secHeading='about me'>
        <v-row>
            <v-col md="4">
                <v-img
                    :aspect-ratio="9/9"
                    lazy-src="https://picsum.photos/id/11/10/6"
                    src="https://picsum.photos/id/237/200/300"
                    height="100%"
                ></v-img>
            </v-col>
            <v-col md="8" class="px-6"> 
                <v-simple-table>
                    <template v-slot:default>
                        <tbody>
                            <tr
                            v-for="item in personal_info"
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
                    <h1 class="text-h5 text-capitalize mb-3">i am Someone E. Else and visual designer</h1>
                    <p class="mb-6">Hi! My name is Someone E. Else. I am a Web Developer, and I'm very passionate and dedi my work. With 20 years experience as a professional</p>
                    <v-btn color="primary">hire me </v-btn>
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
            personal_info:[
                {
                    icon: 'mdi-gift',
                    title: 'birthday',
                    info: '02.06.1900',
                },
                {
                    icon: 'mdi-book-open-outline',
                    title: 'study',
                    info: '02.06.1900',
                },
                {
                    icon: 'mdi-earth',
                    title: 'website',
                    info: 'www.dummy.com',
                },
                {
                    icon: 'mdi-pac-man',
                    title: 'interest',
                    info: 'reading',
                },
                {
                    icon: 'mdi-map-marker',
                    title: 'location',
                    info: '402, random location',
                },
            ]   
        }
    }
}
</script>

<style lang="scss">
// .about-section-heading{
//     text-decoration: underline;
// }
</style>