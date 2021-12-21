<template>
    <div class="single-series-container">
        <div class="series-img-container">
            <img :src="SeriesObject.thumb" :alt="SeriesObject.series">
        </div>
        <h2>{{ SeriesObject.series.toUpperCase() }}</h2>
    </div>
</template>

<script>
export default {
    name: 'SingleSeries',
    props: ['SeriesObject']
}
</script>

<style lang="scss" scoped>
    .single-series-container {
        width: calc( (100% / 6) - 20px );
        margin: 0 10px 20px;
        font-family: "Segoe UI", sans-serif;
        overflow: hidden;

        // test
        background-color: darkcyan;
        border: 1px solid red;

        .series-img-container {
            width: 100%;
            height: 200px;
            overflow: hidden;
        }

        h2 {
            font-weight: lighter;
        }
    }
</style>