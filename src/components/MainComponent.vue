<template>
    <main>
        <div class="container text-center py-5">
            <h5 class="text-white"> --> Content goes here <-- </h5>
        </div>
    </main>
</template>

<script>
import { comics } from '@/data/store';
    export default {
        name: 'MainComponent',
        data() {
            return {
                
            }
        },
        mounted() {
            console.log(comics);
        },

    }


</script>

<style lang="scss" scoped>

    @use '../assets/styles/partials/variables' as *;

    main {
        background-color: $backgroundMain;
    }
</style>