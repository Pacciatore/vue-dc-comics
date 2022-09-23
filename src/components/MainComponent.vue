<template>
    <main>

        <!-- Main content -->
        <div class="content container fs-1">
            -->CONTENT GOES HERE&lt;--
        </div>

        <!-- Pre Footer -->
        <div class="pre-footer">

            <div class="container d-flex py-5 justify-content-around align-items-center">

                <!-- Digital Comics -->
                <div>
                    <a href="#">
                        <img class="pre-footer-icon" src="../assets/img/buy-comics-digital-comics.png"
                            alt="digital-comics">
                        <span class="fs-5">Digital Comics</span>
                    </a>
                </div>

                <!-- DC Merchandise -->
                <div>
                    <a href="#">
                        <img class="pre-footer-icon" src="../assets/img/buy-comics-merchandise.png"
                            alt="comics-merchandise">
                        <span class="fs-5">DC Merchandise</span>
                    </a>
                </div>

                <!-- Subscription -->
                <div>
                    <a href="#">
                        <img class="pre-footer-icon" src="../assets/img/buy-comics-subscriptions.png"
                            alt="subscriptions">
                        <span class="fs-5">Subscription</span>
                    </a>
                </div>

                <!-- Comic Shop Locator -->
                <div>
                    <a href="#">
                        <img class="pre-footer-icon" src="../assets/img/buy-comics-shop-locator.png" alt="shop-locator">
                        <span class="fs-5">Comic Shop Locator</span>
                    </a>
                </div>

                <!-- DC Power Visa -->
                <div>
                    <a href="#">
                        <img class="pre-footer-icon svg" src="../assets/img/buy-dc-power-visa.svg" alt="dc-power-visa">
                        <span class="fs-5">DC Power Visa</span>
                    </a>
                </div>

            </div>

        </div>


    </main>
</template>


<script>
export default {
    name: 'MainComponent'
}
</script>


<style scoped lang="scss">
@import './variables.scss';

main {
    min-height: 500px;
    background-color: black;
    color: white;

    // For pre footer temporary position
    position: relative;
}

// Top footer
.pre-footer {
    background-color: $tr-dc-blue;

    // For pre footer temporary position
    position: absolute;
    bottom: 0;
    width: 100%;
}

.pre-footer a {
    color: inherit;
    text-decoration: none;
}

.pre-footer span {
    text-transform: uppercase;
    font-weight: 300;
}

.pre-footer-icon {
    height: 60px;
    padding-right: 10px;
}

.pre-footer-icon.svg {
    width: 70px;
}
</style>