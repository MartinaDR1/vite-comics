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
    </div>
   
</template>


<style lang="scss" scoped>

</style>