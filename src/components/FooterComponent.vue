<template>
    <footer class="fs-5">
        <div class="container">

            <div class="w-50 d-flex">

                <!-- Firt column -->
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
    </footer>
</template>


<script>
export default {
    name: "FooterComponent",
}
</script>


<style scoped lang="scss">
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
</style>