<template>
    <section class="pre-footer">
        <div class="container">
            
            <div v-for="(element, index) in preFooterObject" class="pre-footer-object" :key="index">
                <img class="object-img" :src="require('../assets/img/' + element.img)" alt="">
                <span>{{ element.name }}</span>
            </div>

        </div>
    </section>
</template>

<script>
export default {
    name: "PreFooter",
    data: function() {
        return {
            preFooterObject: {

                digitalComics: {
                    name: 'DIGITAL COMICS',
                    img: 'buy-comics-digital-comics.png'
                },

                dcMerchandise: {
                    name: 'DC MERCHANDISE',
                    img: 'buy-comics-merchandise.png'
                },

                subscription: {
                    name: 'SUBSCRIPTION',
                    img: 'buy-comics-subscriptions.png'
                },

                ComicShop: {
                    name: 'COMIC SHOP LOCATOR',
                    img: 'buy-comics-shop-locator.png'
                },

                dcPowerVisa: {
                    name: 'DC POWER VISA',
                    img: 'buy-dc-power-visa.svg'
                }
            }
        }
    }
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