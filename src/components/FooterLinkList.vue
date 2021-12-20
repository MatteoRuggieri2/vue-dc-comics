<template>
    <section>
        <div class="container">

            <!-- Link list -->
            <div class="link-list">

                <!-- List -->
                <div class="list-container">
                    <div v-for="(element, index) in linkList.comics"  :key="index">

                        <!-- Title List -->
                        <h3>{{ element.title }}</h3>
                        <ul>
                            <li v-for="(element, index) in linkList.comics[index].link"  :key="index">
                                <a href="#">{{ element }}</a>
                            </li>
                        </ul>
                    </div>
                
                </div>

                <!-- List -->
                <div class="list-container">
                    <div v-for="(element, index) in linkList.dc"  :key="index">

                        <!-- Title List -->
                        <h3>{{ element.title }}</h3>
                        <ul>
                            <li v-for="(element, index) in linkList.dc[index].link"  :key="index">
                                <a href="#">{{ element }}</a>
                            </li>
                        </ul>
                    </div>
                </div>

                <!-- List -->
                <div class="list-container">
                    <div v-for="(element, index) in linkList.sites"  :key="index">

                        <!-- Title List -->
                        <h3>{{ element.title }}</h3>
                        <ul>
                            <li v-for="(element, index) in linkList.sites[index].link"  :key="index">
                                <a href="#">{{ element }}</a>
                            </li>
                        </ul>
                    </div>

                </div>
            </div>

            <!-- DC big logo -->
            <div class="big-logo">
                <img src="../assets/img/dc-logo-bg.png" alt="Big DC Logo">
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "FooterLinkList",
    data: function() {
        return {
            linkList: {

                comics: {
                    dcComics: {
                        title: 'DC COMICS',
                        link: ['Characters', 'Comics', 'Movies', 'TV', 'Games', 'Videos', 'News']
                    },

                    shop: {
                        title: 'SHOP',
                        link: ['Shop DC', 'Shop DC Collectibles']
                    }
                },

                dc: {
                    dcList: {
                        title: 'DC',
                        link: ['Terms Of Use', 'Privacy policy (New)', 'Ad Choices', 'Advertising', 'Jobs', 'Subsciptions', 'Talent Workshops', 'CPSC Certificates', 'Ratings', 'Shop Help', 'Contact Us']
                    }
                },

                sites: {
                    sitesList: {
                        title: 'SITES',
                    link: ['DC', 'MAD Magazine', 'DC Kids', 'DC Universe', 'DC Power Visa']
                    }
                }

            }
        };
    }
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

    section {
        padding: 50px 0;
        color: $secondary_color;
        background-image: url(../assets/img/footer-bg.jpg);
        overflow: hidden;

        .container {
            
            position: relative;

            .link-list{
                display: flex;

                .list-container {
                    margin: 0 20px;

                    ul {
                        margin-bottom: 20px;

                        li {
                            color: grey;
                        }
                    }
                }
            }

            .big-logo {
                position: absolute;
                top: 50%;
                right: 0;
                transform: translateY(-50%);
            }
        }
    }
</style>