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
import FooterBottom from './FooterComponents/FooterBottom.vue';

    export default {
        name: 'FooterComponent',
        components: {
            FooterTop,
            FooterMid,
            FooterBottom,
        }
    };
</script>

<style lang="scss" scoped>
    /* Add your footer styles here */
</style>