<script>
export default {
    data() {
        return {
            name: 'SiteFooter'
        }
    }
}
</script>

<template>
    <footer>
        <div class="top">
            <div class="ms_container d-flex justify-content-between">
                <div class="row py-3">
                    <div class="col-4">
                        <h4 class="py-2">dc comincs</h4>
                        <ol>
                            <li>Characters</li>
                            <li>Comics</li>
                            <li>Movies</li>
                            <li>Tv</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li>
                        </ol>

                        <h4 class="py-2">shop</h4>
                        <ol>
                            <li>Shop DC</li>
                            <li>Shop DC Collectibles</li>
                        </ol>
                    </div>

                    <div class="col-4">
                        <h4 class="py-2">dc </h4>
                        <ol>
                            <li>Terms Of Use</li>
                            <li>Privacy policy (New)</li>
                            <li>Ad Choices</li>
                            <li>Advertiding</li>
                            <li>Jobs</li>
                            <li>Subscriptions</li>
                            <li>Talent Workshops</li>
                            <li>CPSC Certificates</li>
                            <li>Ratings</li>
                            <li>Shop Help</li>
                            <li>Contact Us</li>
                        </ol>
                    </div>

                    <div class="col-4">
                        <h4 class="py-2">sites </h4>
                        <ol>
                            <li>DC</li>
                            <li>MAD Magazfa-inverse</li>
                            <li>DC Kids</li>
                            <li>DC Universe</li>
                            <li>DC Power Visa</li>
                        </ol>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
    @use "../assets/partials/SiteFooter.scss" as *;
</style>