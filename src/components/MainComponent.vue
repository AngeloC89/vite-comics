<template>
    <main>
        <div class="container text-center">
            <h2 class="text-white text-uppercase ">current series</h2>
            <div class="row">
                <div class="col-12 col-md-3 col-lg-2" v-for="(item, index) in comics" :key="index" >
                    <CardComponent :image="item.thumb" :series="item.series" :price="item.price"/>
                </div>
            </div>
        </div>
    </main>
</template>

<script>
    import CardComponent from './MainComponent/CardComponent.vue';
    import { comics } from '../data/store';
    export default {
        name: 'MainComponent',
        components: {
            CardComponent
        },
        data() {
            return {
                comics

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

        h2{
            background-color: $backgroundFooterTop;
            padding: 10px 0px;
            width: 300px;
            margin-right: auto;
            transform: translateY(-50%);
        }
        
    }
   
</style>