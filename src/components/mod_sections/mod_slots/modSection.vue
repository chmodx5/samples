<template>
    <div class="about-section py-12" >
        <v-container>
            <h1 class="text-capitalize about-section-heading text-h3 mb-6">
                {{ secHeading }}
            </h1>
                <slot></slot>
        </v-container>
    </div>
</template>

<script>
export default {
    name: 'modSection',
    props:{
        secHeading: String,
    }
}
</script>