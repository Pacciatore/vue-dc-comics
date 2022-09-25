<template>
    <main>

        <div class="jumbotron"></div>

        <!-- Main content -->
        <div class="main-content position-relative container">

            <div class="group-tag position-absolute fs-1 pt-1">Current Series</div>

            <div class="container pt-5">
                <ComicCardsComponent />
            </div>

        </div>

    </main>
</template>


<script>
import ComicCardsComponent from '@/components/ComponentsUtils/ComicCardsComponent.vue';
export default {
    name: "MainComponent",
    components: { ComicCardsComponent }
}
</script>


<style scoped lang="scss">
@import '@/components/style/variables.scss';

main {
    min-height: 500px;
    background-color: black;
    color: white;
}

.jumbotron {
    background-image: url(@/assets/img/jumbotron.jpg);
    background-size: cover;
    background-position: top;

    height: 400px;
}

.main-content {
    min-height: 300px;

    .group-tag {
        transform: translate(0, -50%);

        background-color: $tr-dc-blue;
        color: white;

        padding: 0 40px;

        text-transform: uppercase;
    }


}
</style>