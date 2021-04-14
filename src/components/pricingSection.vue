<template>
    <div class="my-6">
        <v-container>
            <div class="text-center py-6">
                <h3 class="text-capitalize text-h4">see our prices</h3>
                <p class="my-6">
                    <v-btn color="primary" class="mx-3">annually</v-btn>
                    <v-btn class="mx-3">monthly</v-btn>
                </p>
            </div>
            <v-row>
                <v-col v-for="pricing in pricing" :key="pricing.id">
                    <v-card class="text-center px-3 py-6" :class="{ primary: pricing.is_primary , 'white--text': pricing.is_primary }">
                        <p class="font-weight-bold text-h6 text-capitalize"> {{pricing.title}} </p>
                        <p class="text-h4"> 
                            <span>$</span>
                            {{ pricing.price }}
                        </p>
                        <p class="my-6"> {{ pricing.desc }} </p>
                        <p>
                            <v-btn v-if="pricing.is_primary" color="white" :to="pricing.link" > check out </v-btn>
                            <v-btn v-else :to="pricing.link" color="primary"> check out </v-btn>
                        </p>
                    </v-card>
                </v-col>
            </v-row>
        </v-container>
    </div>
</template>

<script>
export default {
    name: 'pricingSection',
    data(){
        return{
            pricing: [
                {
                    title: 'amateur',
                    is_primary: false,
                    price: '40',
                    desc: 'this is all i could think of',
                    link: '/'
                },
                {
                    title: 'professional',
                    is_primary: true,
                    price: '60',
                    desc: 'this is all i could think of',
                    link: '/'
                },
                {
                    title: 'enterpice',
                    is_primary: false,
                    price: '80',
                    desc: 'this is all i could think of',
                    link: '/'
                },
            ]
        }
    }
}
</script>