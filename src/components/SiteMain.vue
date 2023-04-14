<script>
import banner from "../data/banner";
import ComicsList from "../components/ComicsList.vue";
export default {
    data() {
        return {
            name: 'SiteMain',
            banner: banner,
            ComicsList:ComicsList
        }
    },
    components: {
        banner,
        ComicsList
    },
}
</script>

<template>
    <main>
        <div class="jumbo"></div>

        <div class="container py-5">
            <ComicsList/>
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