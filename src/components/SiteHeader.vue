<script>
import navBar from "../data/navBar";
export default {
    data() {
        return {
            name: 'SiteHeader',
            navBar: navBar,
            activeLink: 1,
        }
    },
    components: {
        navBar,
    },
}
</script>

<template>
    <header>
        <div class="container my-3">
            <div class="row">
                <div class="col d-flex justify-content-between">
                    <div class="logo">
                        <img style="width: 65px;" src="../assets/img/dc-logo.png" alt="">
                    </div>

                    <div class="nav d-flex align-items-center ">
                        <ul class="d-flex">
                            <li :class="link === activeLink ? 'active' : ''" v-for="(item, link) in navBar"> 
                                <a :href="item.link" >{{ item.text }}</a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>
@use "../assets/partials/variables" as *;

    .active{
        padding-bottom: 1rem;
        border-bottom: 4px solid $accent;
    }

    li:hover{
        border-bottom: 4px solid $accent;
        cursor: pointer;
    }

  
</style>