<template>
    <section>
        <div class="container">
            <a class="btn-blue-border" href="#">SIGN-UP NOW!</a>
            <div class="socials-container">
                <span class="follow-us">FOLLOW US</span>

                <ul>
                    <li v-for="(element, index) in socials" :key="index">
                        <a href="#"><img class="social-icon" :src="require('../assets/img/' + element.img)" :alt="element.name"></a>
                    </li>
                </ul>
                
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "FooterSocials",
    data: function() {
        return {
            socials: {

                digitalComics: {
                    name: 'facebook',
                    img: 'footer-facebook.png'
                },

                dcMerchandise: {
                    name: 'twitter',
                    img: 'footer-twitter.png'
                },

                subscription: {
                    name: 'youtube',
                    img: 'footer-youtube.png'
                },

                ComicShop: {
                    name: 'pinterest',
                    img: 'footer-pinterest.png'
                },

                dcPowerVisa: {
                    name: 'periscope',
                    img: 'footer-periscope.png'
                }
            }
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';
@import '../style/general.scss';

    section {
        padding: 40px 0;
        background-color: #303030;
        color: $secondary_color;
        
        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;

            .socials-container {
                display: flex;
                align-items: center;

                .follow-us {
                    color: $primary_color;
                }

                ul {
                    margin-left: 20px;
                    display: flex;
                }
            }

            .social-icon {
                width: 40px;
                margin: 0 10px;
            }
        }

    }
</style>