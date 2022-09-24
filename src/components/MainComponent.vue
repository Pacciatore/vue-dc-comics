<template>
    <main>

        <div class="jumbotron"></div>

        <!-- Main content -->
        <div class="main-content container fs-1">
            -->CONTENT GOES HERE&lt;--
        </div>

    </main>
</template>


<script>
export default {
    name: "MainComponent",
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
}
</style>