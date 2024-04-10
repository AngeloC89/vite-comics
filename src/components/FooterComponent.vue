<template>
    <footer>
        <FooterTop />
        <FooterMid />
        <FooterBottom />
    </footer>
</template>

<script>
import FooterTop from './FooterComponents/FooterTop.vue';
import FooterMid from './FooterComponents/FooterMid.vue';

    export default {
        name: 'FooterComponent',
        components: {
            FooterTop,
            FooterMid,
        }
    };
</script>

<style lang="scss" scoped>
    /* Add your footer styles here */
</style>