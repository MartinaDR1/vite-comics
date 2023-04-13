<script>
import banner from "../data/banner";
export default {
    data() {
        return {
            name: 'SiteMain',
            banner: banner,
        }
    },
    components: {
        banner,
    },
}
</script>

<template>
    <main>
        <div class="container py-5">
            <span>Content goes here</span> 
        </div>

        <div class="banner py-5">
            <div class="container">
                <div class="row">
                    <div class="col d-flex gap-3 justify-content-center align-items-center" v-for="item in banner">
                        <img :src="item.icon" alt="">
                        <span class="px-2">{{ item.text }}</span>
                    </div>
                </div>
            </div>
        </div>
    </main>
</template>

<style lang="scss" scoped>
    @use "../assets/partials/SiteMain.scss" as *;
</style>