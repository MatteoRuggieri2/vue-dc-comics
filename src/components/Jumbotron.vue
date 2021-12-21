<template>
    <section class="jumbotron">
        <img class="jumbo-img" src="../assets/img/jumbotron.jpg" alt="Jumbotron">
    </section>
</template>

<script>
export default {
    name: 'Jumbotron'
}
</script>

<style lang="scss" scoped>
    .jumbotron {
        width: 100%;
        height: 400px;

        .jumbo-img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: center top;
        }
    }
</style>