<template>
    <footer class="fs-5">

        <!-- Main footer -->
        <div class="container">

            <div class="w-50 d-flex py-5">

                <!-- First column -->
                <div class="col-4">
                    <ul>
                        <li class="fs-3">DC Comics</li>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>

                    <ul>
                        <li>Shop</li>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>
                    </ul>
                </div>

                <!-- Second column -->
                <div class="col-4">
                    <ul>
                        <li>DC</li>
                        <li>Terms of Use</li>
                        <li>Privacy policy (New)</li>
                        <li>Ad Choices</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>Talent Workshops</li>
                        <li>CPSC Certificates</li>
                        <li>Ratings</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>
                </div>

                <!-- Third column -->
                <div class="col-4">
                    <ul>
                        <li>Sites</li>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa</li>
                    </ul>
                </div>

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

    min-height: 250px;
}

ul {
    list-style-type: none;
}

li:first-child {
    color: white;
    font-weight: 400;
    text-transform: uppercase;
}

li {
    color: #ffffff5f;
    font-weight: 300;
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
}

.social-invite {
    color: $tr-dc-blue;
}

.social-link:hover {
    filter: brightness(50);
}
</style>