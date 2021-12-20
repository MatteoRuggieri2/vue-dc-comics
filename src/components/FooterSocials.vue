<template>
    <section>
        <div class="container">
            <a class="btn-blue-border" href="#">SIGN-UP NOW!</a>
            <div class="socials-container">
                <span class="follow-us">FOLLOW US</span>

                <ul>
                    <li>
                        <a href="#"><img class="social-icon" src="../assets/img/footer-facebook.png" alt="facebook icon"></a>
                    </li>

                    <li>
                        <a href="#"><img class="social-icon" src="../assets/img/footer-twitter.png" alt="twitter icon"></a>
                    </li>

                    <li>
                        <a href="#"><img class="social-icon" src="../assets/img/footer-youtube.png" alt="youtube icon"></a>
                    </li>

                    <li>
                        <a href="#"><img class="social-icon" src="../assets/img/footer-pinterest.png" alt="pinterest icon"></a>
                    </li>

                    <li>
                        <a href="#"><img class="social-icon" src="../assets/img/footer-periscope.png" alt="periscope icon"></a>
                    </li>
                </ul>
                
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "FooterSocials"
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';
@import '../style/general.scss';

    section {
        padding: 40px 0;
        background-color: #303030;
        color: white;
        
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