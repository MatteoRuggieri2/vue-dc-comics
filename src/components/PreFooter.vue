<template>
    <section class="pre-footer">
        <div class="container">
            
            <div class="pre-footer-object">
                <img class="object-img" src="../assets/img/buy-comics-digital-comics.png" alt="digital comics">
                <span>DIGITAL COMICS</span>
            </div>

            <div class="pre-footer-object">
                <img class="object-img" src="../assets/img/buy-comics-digital-comics.png" alt="dc merchandise">
                <span>DIGITAL COMICS</span>
            </div>

            <div class="pre-footer-object">
                <img class="object-img" src="../assets/img/buy-comics-digital-comics.png" alt="subscription">
                <span>DIGITAL COMICS</span>
            </div>

            <div class="pre-footer-object">
                <img class="object-img" src="../assets/img/buy-comics-digital-comics.png" alt="comic shop locator">
                <span>DIGITAL COMICS</span>
            </div>

            <div class="pre-footer-object">
                <img class="object-img" src="../assets/img/buy-comics-digital-comics.png" alt="dc power visa">
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
        vertical-align: middle;
    }

    .object-img {
        width: 50px;
        margin-right: 10px;
        vertical-align: middle;
    }
</style>