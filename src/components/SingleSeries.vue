<template>
    <div class="single-series-container">
        <a href="#">
            <div class="series-img-container">
                <img :src="SeriesObject.thumb" :alt="SeriesObject.series">
            </div>
            <h2>{{ SeriesObject.series.toUpperCase() }}</h2>
        </a>
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
        width: calc( (100% / 6) - 30px );
        margin: 10px 15px;
        overflow: hidden;

        .series-img-container {
            width: 100%;
            height: 200px;
            overflow: hidden;
        }

        h2 {
            padding: 20px 0;
            font-family: "Segoe UI", sans-serif;
            font-weight: lighter;
            font-size: 16px;
        }
    }
</style>