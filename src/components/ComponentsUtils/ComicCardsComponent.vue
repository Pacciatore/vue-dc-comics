<template>
    <div class="comic-container d-flex flex-wrap pt-3 g-0">

        <div v-for="(comic, index) in comics" :key="index" class="col-2">

            <!-- Comic thumb -->
            <div class="comic-thumb position-relative me-2">

                <!-- Displays on hover -->
                <div class="comic-info pe-2 position-absolute d-flex flex-column align-items-end justify-content-end">
                    <div class="comic-type text-capitalize">{{ comic.type }}</div>
                    <div class="comic-price fs-5">{{ comic.price }}</div>
                </div>

                <!-- Comic image -->
                <img class="img-fluid" :src="comic.thumb" :alt="comic.series">

            </div>

            <!-- Comic Series display -->
            <div class="comic-series text-uppercase fs-5 py-3">
                {{ comic.series }}
            </div>

        </div>

    </div>
</template>

<script>
export default {
    name: 'ComicCards',
    props: {
        comics: Array
    },
}
</script>

<style lang="scss" scoped>
@import '@/assets/style/variables.scss';

.comic-container {

    row-gap: 2rem;

    cursor: default;

    .comic-thumb {
        overflow-y: hidden;
        height: 200px;

        .comic-info {
            height: 100%;
            width: 100%;

            // Uso di colori rgba per permettere l'hover
            background-color: rgba(0, 0, 0, 0);
            color: rgba(255, 255, 255, 0);

            transition: all $tr-hover-transition;

            cursor: pointer;

            &:hover {
                background-color: rgba(0, 0, 0, 0.5);
                color: rgba(255, 255, 255, 1);
            }
        }

    }

    .comic-series {
        font-weight: 300;
        line-height: 1.25rem;
    }
}
</style>