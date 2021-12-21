<template>
    <div>
        <h2>{{ SeriesTitle }}</h2>
        <h2></h2>
        <h2></h2>
    </div>
</template>

<script>
export default {
    name: 'SingleSeries',
    props: ['ImgSrc', 'ImgAlt', 'SeriesTitle']
}
</script>