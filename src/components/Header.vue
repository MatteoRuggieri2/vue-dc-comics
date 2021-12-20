<template>
    <header>
        <div class="container">

            <!-- Logo -->
            <div class="logo-container">
                <img src="../assets/img/dc-logo.png" alt="DC Logo">
            </div>
            
            <!-- Link list -->
            <ul>
                <li v-for="(element, index) in headerLink" :key="index">
                    <a href="#">{{ element }}</a>
                </li>
            </ul>
        </div>
    </header>
</template>

<script>
export default {
    name: "Header",
    data: function() {
        return{
            headerLink: ['characters', 'comics', 'movies', 'tv', 'games', 'collectibles', 'videos', 'fans', 'news', 'shop']
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
            display: flex;
            justify-content: space-between;
            align-items: center;
            height: 100%;

        }

        ul {
            li {
                display: inline-block;
                line-height: 116px;
                padding-bottom: 4px;
                text-transform: uppercase;

                &:hover {
                    color: $primary_color;
                    border-bottom: 4px solid $primary_color;
                    padding-bottom: 0px;
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