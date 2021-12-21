<template>
    <div class="container">
        <span class="main-title">CURRENT SERIES</span>
    </div>
</template>

<script>
export default {
    name: "MainContent"
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

    .container {
        padding: 50px 0;
        position: relative;

        .main-title {
            padding: 8px 30px;
            font-size: 30px;
            color: $secondary_color;
            background-color: $primary_color;
            position: absolute;
            top: 0;
            left: 0;
            transform: translateY(-50%);
        }
    }

</style>