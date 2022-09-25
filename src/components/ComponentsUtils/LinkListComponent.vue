<template>

    <ul>
        <li class="fs-3">{{ listArray.title }}</li>
        <li v-for="liElement in listArray.elements" :key="liElement">
            <a href="#">{{ liElement }}</a>
        </li>
    </ul>

</template>

<script>
export default {
    name: 'LinkList',
    props: {
        listArray: Object
    }

}
</script>

<style scoped lang="scss">

</style>