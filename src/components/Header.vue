<template>
    <header>
        <div class="container">

            <div class="wrapper">
                <!-- Logo -->
                <div class="logo-container">
                    <img src="../assets/img/dc-logo.png" alt="DC Logo">
                </div>
                
                <!-- Link list -->
                <ul>
                    <li v-for="(element, index) in headerLink" :key="index" :class="{ selected: element.selectedPage }">
                        <a href="element.url">{{ element.text }}</a>
                    </li>
                </ul>
            </div>

        </div>
    </header>
</template>

<script>
export default {
    name: "Header",
    data: function() {
        return{
            headerLink: [
                
                {
                    text: 'characters',
                    url: '#',
                    selectedPage: false
                },

                {
                    text: 'comics',
                    url: '#',
                    selectedPage: true
                },

                {
                    text: 'movies',
                    url: '#',
                    selectedPage: false
                },

                {
                    text: 'tv',
                    url: '#',
                    selectedPage: false
                },

                {
                    text: 'games',
                    url: '#',
                    selectedPage: false
                },

                {
                    text: 'collectibles',
                    url: '#',
                    selectedPage: false
                },

                {
                    text: 'videos',
                    url: '#',
                    selectedPage: false
                },

                {
                    text: 'fans',
                    url: '#',
                    selectedPage: false
                },

                {
                    text: 'news',
                    url: '#',
                    selectedPage: false
                },

                {
                    text: 'shop',
                    url: '#',
                    selectedPage: false
                }
                
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import '../style/variables.scss';

    header{
        width: 100%;
        height: 120px;
    
        .container {
            .wrapper {
                display: flex;
                justify-content: space-between;
                align-items: center;
                height: 100%;

            }
        }

        ul {
            li {
                display: inline-block;
                line-height: 116px;
                padding-bottom: 4px;
                text-transform: uppercase;

                &.selected {
                    color: $primary_color;
                    border-bottom: 4px solid $primary_color;
                    padding-bottom: 0px;
                }

                &:hover {
                    color: darken($primary_color, 10%);
                }
                
                a {
                    margin: 0 20px;
                    font-size: 14px;
                }
            }
        }
    }

    .logo-container {
        width: 80px;
    }
</style>