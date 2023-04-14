<script>
    import comics from "../data/dc-comics.json";
    import ComicsItem from "./ComicsItem.vue";

    export default {
        components: {
             ComicsItem
        },
        data(){
            return{
                comics: comics,
            }
        }
    }
</script>


<template>
    <div class="container">
        <div class="row">
            <ComicsItem v-for="ComicsItem in comics" 
            :thumb="ComicsItem.thumb" 
            :series="ComicsItem.series" 
            :price="ComicsItem.price" 
            :type="ComicsItem.type"/>
        </div>


        <button class="btn">Load more</button>
    </div>
   
</template>


<style lang="scss" scoped>
    @use '../assets/partials/variables' as *;

    .container{
        text-align: center;
    }
    button{
        background-color: $accent;
        color: $primary;
        text-transform: uppercase;
        padding: 0.7rem 2rem;
        align-self: center;
        border: none;
    }
</style>