<template>
    <FooterMerch />
    <FooterLinks />
    <FooterIcon />
</template>

<script>
import FooterMerch from './FooterMerch.vue';
import FooterLinks from './FooterLinks.vue';
import FooterIcon from './FooterIcon.vue';
    export default {
        name : 'FooterDc',
        components :{
            FooterMerch,
            FooterLinks,
            FooterIcon
        }
    }
</script>

<style lang="scss" scoped>

</style>