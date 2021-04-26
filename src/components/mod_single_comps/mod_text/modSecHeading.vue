<template>
    <h1 class="text-capitalize about-section-heading text-h3 mb-6">
        {{ text }}
    </h1>
</template>
<script>
export default {
    name: 'modSecHeading',
    props: {
        text: String
    }
}
</script>