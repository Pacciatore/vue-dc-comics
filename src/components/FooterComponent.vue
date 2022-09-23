<template>
    <footer class="fs-5">

        <!-- PreFooter Component Reference -->
        <PreFooterComponent />

        <!-- Main footer -->
        <div class="main-footer">
            <div class="container d-flex justify-content-between">

                <!-- Footer Links -->
                <div class="col-4 d-flex py-4">

                    <!-- First column -->
                    <div class="col-4">
                        <ul>
                            <li class="fs-3">DC Comics</li>
                            <li> <a href="#">Characters</a></li>
                            <li> <a href="#">Comics</a></li>
                            <li> <a href="#">Movies</a></li>
                            <li> <a href="#">TV</a></li>
                            <li> <a href="#">Games</a></li>
                            <li> <a href="#">Videos</a></li>
                            <li> <a href="#">News</a></li>
                        </ul>

                        <ul>
                            <li class="fs-3">Shop</li>
                            <li> <a href="#">Shop DC</a></li>
                            <li> <a href="#">Shop DC Collectibles</a></li>
                        </ul>
                    </div>

                    <!-- Second column -->
                    <div class="col-4">
                        <ul>
                            <li class="fs-3">DC</li>
                            <li> <a href="#">Terms of Use</a></li>
                            <li> <a href="#">Privacy policy (New)</a></li>
                            <li> <a href="#">Ad Choices</a></li>
                            <li> <a href="#">Advertising</a></li>
                            <li> <a href="#">Jobs</a></li>
                            <li> <a href="#">Subscriptions</a></li>
                            <li> <a href="#">Talent Workshops</a></li>
                            <li> <a href="#">CPSC Certificates</a></li>
                            <li> <a href="#">Ratings</a></li>
                            <li> <a href="#">Shop Help</a></li>
                            <li> <a href="#">Contact Us</a></li>
                        </ul>
                    </div>

                    <!-- Third column -->
                    <div class="col-4">
                        <ul>
                            <li class="fs-3">Sites</li>
                            <li> <a href="#">DC</a></li>
                            <li> <a href="#">MAD Magazine</a></li>
                            <li> <a href="#">DC Kids</a></li>
                            <li> <a href="#">DC Universe</a></li>
                            <li> <a href="#">DC Power Visa</a></li>
                        </ul>
                    </div>

                </div>

                <!-- Logo nel background -->
                <div class="dc-footer-mark col-6">
                </div>

            </div>
        </div>

        <!-- BottomFooter Component Reference -->
        <BottomFooterComponent />

    </footer>
</template>


<script>
import BottomFooterComponent from './BottomFooterComponent.vue';
import PreFooterComponent from './PreFooterComponent.vue';
export default {
    name: "FooterComponent",
    components: { BottomFooterComponent, PreFooterComponent }
}
</script>


<style scoped lang="scss">
@import './variables.scss';

// Main footer
.main-footer {
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;

    color: white;

    // Lista link
    ul {
        list-style-type: none;

        // Titolo lista
        li:first-child {
            color: white;
            font-weight: 400;
            text-transform: uppercase;

            cursor: default;
        }

        // Elementi lista
        li a {
            text-decoration: none;
            color: #ffffff5f;
            font-weight: 300;

            transition: color 0.25s;


            &:hover {
                color: $tr-dc-blue;
            }

        }


    }

    // Logo DC in background
    .dc-footer-mark {
        background-image: url(../assets/img/dc-logo-bg.png);
        background-position: center;
        background-repeat: no-repeat;
        background-size: auto;
    }

}
</style>