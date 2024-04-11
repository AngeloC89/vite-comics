<template>
    <main>
        <div class="container text-center">
            <h2 class="text-white text-uppercase ">current series</h2>
            <div class="row">
                <div id="card" class="col-12 col-md-3 col-lg-2" v-for="(item, index) in comics" :key="index">
                    <CardComponent :image="item.thumb" :series="item.series" :price="item.price"
                        @remove="removeCard(index)" />
                </div>
            </div>
            <div class="btn btn-primary text-uppercase w-25 my-5 m-auto ">load more</div>
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
        methods: {
            removeCard(index) {
                this.comics.splice(index, 1);

            },
            mounted() {

            },

        }
    }


</script>

<style lang="scss" scoped>

    @use '../assets/styles/partials/variables' as *;

    main {
        background-color: $backgroundMain;

        h2 {
            background-color: $backgroundFooterTop;
            padding: 10px 0px;
            width: 300px;
            margin-right: auto;
            transform: translateY(-50%);
        }

        #card {

            margin-bottom: 20px;
            transition: 0.5s;


            &:hover {
                transform: scale(1.1);

                opacity: 0.5;
            }
        }
    }

</style>