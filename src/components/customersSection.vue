<template>
<div class="text-center my-6">
    <v-container>
        <h3 class="te text-capitalize text-h4 mb-3">what out customers are saying</h3>
        <v-row>
            <v-col v-for="i in 2" :key="i">
                <v-card class="pa-6">
                    <div class="d-flex justify-center mb-3">
                        <span>
                            <v-img src="../assets/WarthogHead.svg" :aspect-ratio="1/1" width="100">
                            </v-img>
                        </span>
                    </div>
                    
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolor aut molestias ullam excepturi quos deserunt perspiciatis, mollitia voluptates consequuntur! Doloremque, vel impedit. Tempora, voluptatum recusandae fugit culpa, eum voluptatibus, tenetur.!</p>
                </v-card>
            </v-col>
            
        </v-row>
    </v-container>
</div>
</template>

<script>
export default {
    name: 'customersSection',
    data(){
        return{

        }
    }
}
</script>