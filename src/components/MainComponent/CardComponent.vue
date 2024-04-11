<template>
    <div>
        <div class="card-img">
            <img :src="image" class="img-fluid w-100 " :alt="series">
        </div>
        <div class="card-body text-start decription my-2">
            <h5 class="text-white">{{ series }}</h5>
        </div>
    </div>
    <div class="d-flex align-items-end justify-content-between">
        <span class="text-white ">{{ price }}</span>
        <a class="btn btn-primary mx-3 text-uppercase text-decoration-none" href="#"
            @click="$emit('remove')">Remove</a>
    </div>
</template>

<script>
    export default {
        name: 'CardComponent',
        props: [
            'image',
            'series',
            'price',
            'link'
        ],



    }
</script>



<style lang="scss" scoped>

    img {
        min-height: 300px;

    }
    .decription{
        height: 50px;
    }


</style>