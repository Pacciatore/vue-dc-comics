<template>
    <div class="bottom-footer py-4">
        <div class="container d-flex justify-content-between">

            <button class="sign-up-btn py-2 px-3 fs-4">Sign-Up Now!</button>

            <div class="socials col-4 d-flex align-items-center justify-content-around">
                <div class="social-invite text-uppercase fs-3">Follow us</div>
                <a href="#" class="social-link"><img src="@/assets/img/footer-facebook.png" alt=""></a>
                <a href="#" class="social-link"><img src="@/assets/img/footer-twitter.png" alt=""></a>
                <a href="#" class="social-link"><img src="@/assets/img/footer-youtube.png" alt=""></a>
                <a href="#" class="social-link"><img src="@/assets/img/footer-pinterest.png" alt=""></a>
                <a href="#" class="social-link"><img src="@/assets/img/footer-periscope.png" alt=""></a>
            </div>

        </div>
    </div>
</template>

<script>
export default {
    name: 'BottomFooterComponent',
}
</script>

<style scoped lang="scss">
@import '@/assets/style/variables.scss';

// Bottom footer
.bottom-footer {
    background-color: $tr-dc-bg-bottom-footer;
}

.sign-up-btn {
    background-color: inherit;
    color: white;

    text-transform: uppercase;
    border: 2px solid $tr-dc-blue;

    transition: all $tr-hover-transition;
}

.sign-up-btn:hover {
    color: $tr-dc-blue;
    border-color: white;
}

.social-invite {
    color: $tr-dc-blue;
    cursor: default;
}

.social-link:hover {
    filter: brightness(50);
}
</style>