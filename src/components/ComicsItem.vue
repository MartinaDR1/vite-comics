<script>
    export default {
        name: 'ComicsItem',

        props: {
        thumb: String,
        price: String,
        series: String, 
        type: String
        },  

    }
</script>


<template>
   <div class="col py-3">
        <div class="image">
            <img :src="thumb" :alt="series">
        </div>
        <h6 class="my-2">{{series}}</h6>

    </div>
</template>


<style lang="scss" scoped>
    img {
        height: 150px;
        width: 150px;
    }

    h6{
        text-transform: uppercase;
        color: white;
    }
</style>