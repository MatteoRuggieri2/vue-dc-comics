<template>
    <section class="pre-footer">
        <div class="container">
            
            <div class="pre-footer-object">
                <img class="img23" src="../assets/img/buy-comics-digital-comics.png" alt="">
                <span>DIGITAL COMICS</span>
            </div>

            <div class="pre-footer-object">
                <img class="img23" src="../assets/img/buy-comics-digital-comics.png" alt="">
                <span>DIGITAL COMICS</span>
            </div>

            <div class="pre-footer-object">
                <img class="img23" src="../assets/img/buy-comics-digital-comics.png" alt="">
                <span>DIGITAL COMICS</span>
            </div>

            <div class="pre-footer-object">
                <img class="img23" src="../assets/img/buy-comics-digital-comics.png" alt="">
                <span>DIGITAL COMICS</span>
            </div>

            <div class="pre-footer-object">
                <img class="img23" src="../assets/img/buy-comics-digital-comics.png" alt="">
                <span>DIGITAL COMICS</span>
            </div>

        </div>
    </section>
</template>

<script>
export default {
    name: "PreFooter"
}
</script>

<style lang="scss" scoped>
    .pre-footer {
        width: 100%;
        padding: 50px 0;
        background-color: #0282f9;
        color: white;

        .container {
            display: flex;
            justify-content: space-around;
        }
    }

    .pre-footer-object {
        background-color: violet;
        vertical-align: middle;
    }

    .img23 {
        width: 50px;
        margin-right: 10px;
        vertical-align: middle;
    }
</style>