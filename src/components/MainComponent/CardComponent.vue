<template>
    <div>
        <div>
            <img :src="image" class="img-fluid w-100 " :alt="series">
        </div>
        <div class="card-body mt-3">
            <h5 class="text-white">{{ series }}</h5>
            <span>{{ price }}</span>
        </div>

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

img{
    min-height: 300px;
}


</style>