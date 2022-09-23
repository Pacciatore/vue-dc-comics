<template>
    <main>

        <!-- Main content -->
        <div class="content container fs-1">
            -->CONTENT GOES HERE&lt;--
        </div>

        <!-- PreFooterComponent Reference -->
        <PreFooterComponent />

    </main>
</template>


<script>
import PreFooterComponent from './PreFooterComponent.vue';
export default {
    name: "MainComponent",
    components: { PreFooterComponent }
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
</style>