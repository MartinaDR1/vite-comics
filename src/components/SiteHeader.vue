<script>
import navBar from "../data/navBar";
export default {
    data() {
        return {
            name: 'SiteHeader',
            navBar: navBar,
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
                        <ul>
                            <li>
                                <a href="" v-for="item in navBar">{{item.text }}</a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </header>
</template>

<style></style>