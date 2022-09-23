<template>
    <footer class="fs-5">

        <!-- Main footer -->
        <div class="container d-flex justify-content-between">

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

            <div class="dc-footer-mark col-6">
            </div>

        </div>

        <!-- Bottom footer -->
        <div class="bottom-footer py-4">
            <div class="container d-flex justify-content-between">

                <button class="sign-up-btn py-2 px-3 fs-4">Sign-Up Now!</button>

                <div class="socials col-4 d-flex align-items-center justify-content-around">
                    <div class="social-invite text-uppercase fs-3">Follow us</div>
                    <a href="#" class="social-link"><img src="../assets/img/footer-facebook.png" alt=""></a>
                    <a href="#" class="social-link"><img src="../assets/img/footer-twitter.png" alt=""></a>
                    <a href="#" class="social-link"><img src="../assets/img/footer-youtube.png" alt=""></a>
                    <a href="#" class="social-link"><img src="../assets/img/footer-pinterest.png" alt=""></a>
                    <a href="#" class="social-link"><img src="../assets/img/footer-periscope.png" alt=""></a>
                </div>

            </div>
        </div>

    </footer>
</template>


<script>
export default {
    name: "FooterComponent",
}
</script>


<style scoped lang="scss">
@import './variables.scss';

// Main footer
footer {
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;

    color: white;
}

ul {
    list-style-type: none;
}

li:first-child {
    color: white;
    font-weight: 400;
    text-transform: uppercase;
}

li a {
    text-decoration: none;
    color: #ffffff5f;
    font-weight: 300;

    transition: color 0.25s;
}

li a:hover {
    color: $tr-dc-blue;
}

.dc-footer-mark {
    background-image: url(../assets/img/dc-logo-bg.png);
    background-position: center;
    background-repeat: no-repeat;
    background-size: auto;
}

// Bottom footer
.bottom-footer {
    background-color: $tr-dc-bg-bottom-footer;
}

.sign-up-btn {
    background-color: inherit;
    color: white;

    text-transform: uppercase;
    border: 2px solid $tr-dc-blue;

    transition: all 0.25s;
}

.sign-up-btn:hover {
    color: $tr-dc-blue;
    border-color: white;
}

.social-invite {
    color: $tr-dc-blue;
}

.social-link:hover {
    filter: brightness(50);
}
</style>