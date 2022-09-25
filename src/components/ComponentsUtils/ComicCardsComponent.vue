<template>

    <div class="comic-container d-flex flex-wrap pt-3 g-0">

        <div v-for="(comic,index) in comics" :key="index" class="col-2">

            <div class="comic-img-container">
                <img class="img-fluid" :src="comic.thumb" :alt="comic.series">
            </div>

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
.comic-container {

    row-gap: 2rem;

    cursor: default;

    .comic-img-container {
        overflow-y: hidden;
        height: 200px;
    }

    .comic-series {
        font-weight: 300;
        line-height: 1.25rem;
    }
}
</style>