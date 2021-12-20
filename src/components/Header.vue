<template>
    <header>
        <div class="container">

            <!-- Logo -->
            <div class="logo-container">
                <img src="../assets/img/dc-logo.png" alt="DC Logo">
            </div>
            
            <!-- Link list -->
            <ul>
                <li><a href="#">characters</a></li>
                <li><a href="#">comics</a></li>
                <li><a href="#">movies</a></li>
                <li><a href="#">tv</a></li>
                <li><a href="#">games</a></li>
                <li><a href="#">collectibles</a></li>
                <li><a href="#">videos</a></li>
                <li><a href="#">fans</a></li>
                <li><a href="#">news</a></li>
                <li><a href="#">shop</a></li>
            </ul>
        </div>
    </header>
</template>

<script>
export default {
    name: "Header"
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
                    margin: 0 10px;
                }
            }
        }
    }

    .logo-container {
        width: 80px;
    }
</style>