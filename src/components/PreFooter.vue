<template>
    <section class="pre-footer">
        <div class="container">
            
            <div class="pre-footer-object">
                <img class="object-img" src="../assets/img/buy-comics-digital-comics.png" alt="digital comics">
                <span>DIGITAL COMICS</span>
            </div>

            <div class="pre-footer-object">
                <img class="object-img" src="../assets/img/buy-comics-merchandise.png" alt="dc merchandise">
                <span>DC MERCHANDISE</span>
            </div>

            <div class="pre-footer-object">
                <img class="object-img" src="../assets/img/buy-comics-subscriptions.png" alt="subscription">
                <span>SUBSCRIPTION</span>
            </div>

            <div class="pre-footer-object">
                <img class="object-img" src="../assets/img/buy-comics-shop-locator.png" alt="comic shop locator">
                <span>COMIC SHOP LOCATOR</span>
            </div>

            <div class="pre-footer-object">
                <img class="object-img" src="../assets/img/buy-dc-power-visa.svg" alt="dc power visa">
                <span>DC POWER VISA</span>
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
        height: 50px;
        max-width: 60px;
        width: auto;
        margin-right: 10px;
        vertical-align: middle;
    }
</style>