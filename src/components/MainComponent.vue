<template>
    <main>

        <div class="jumbotron"></div>

        <!-- Main content -->
        <div class="main-content position-relative container">

            <!-- Titolo: Current Series -->
            <div class="group-tag position-absolute fs-1 pt-1">Current Series</div>

            <!-- Raccolta: Fumetti attuali -->
            <div class="container pt-5">
                <ComicCardsComponent :comics="currentSeries" />
            </div>

            <!-- Bottone 'carica altri fumetti'
                    Possibile implementazione: ripetizione dell'array per aumentare
                    i fumetti visibili
            -->
            <div class="text-center py-3">
                <button class="group-tag btn rounded-0 fs-5 py-1">
                    Load more
                </button>
            </div>

        </div>

    </main>
</template>


<script>
import ComicCardsComponent from '@/components/ComponentsUtils/ComicCardsComponent.vue';

export default {
    name: "MainComponent",
    components: { ComicCardsComponent },
    props: {
        currentSeries: Array
    }
}
</script>


<style scoped lang="scss">
@import '@/assets/style/variables.scss';

main {
    min-height: 500px;
    background-color: $tr-main-bg-black;
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

        // text: CURRENT SERIES
        &.position-absolute {
            transform: translate(0, -50%);
        }

        // text: LOAD MORE
        // durata transition 0.15s ereditata da .btn di bootstrap
        &.btn:hover {
            color: $tr-dc-black;
            cursor: pointer;
        }

        border: 0;
        background-color: $tr-dc-blue;
        padding: 0 40px;

        text-transform: uppercase;
        color: white;

        cursor: default;
    }


}
</style>