<template>
    <v-footer
        dark
        padless
    >
        <v-card
        class="flex"
        flat
        tile
        >
                <v-card-title class="primary">
                    <v-container class="">
                        <div class="d-flex">
                            <strong class="subheading">Connect with me on social networks!</strong>

                            <v-spacer></v-spacer>

                            <v-btn
                            v-for="icon in icons"
                            :key="icon"
                            class="mx-4"
                            dark
                            icon
                            >
                            <v-icon size="24px">
                                {{ icon }}
                            </v-icon>
                            </v-btn>
                        </div>
                    </v-container>
                </v-card-title>

        <v-card-text class="py-2 white--text text-center">
            {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
        </v-card-text>
        </v-card>
    </v-footer>
</template>

<script>
export default {
    name: 'modFooter',
    data(){
        return{
            icons: [
                'mdi-facebook',
                'mdi-twitter',
                'mdi-linkedin',
                'mdi-instagram',
            ],
        }
    }
}
</script>