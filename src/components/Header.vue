<template>
    <header>
        <div class="container">

            <!-- Logo -->
            <div class="logo-container">
                <img src="../assets/img/dc-logo.png" alt="">
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
    header{
        width: 100%;
        height: 120px;
        /* padding: 20px; */
    

        /* test */
        // background-color: darkcyan;

        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            height: 100%;

            // test
            // background-color: darkgoldenrod;
        }

        ul {
            li {
                display: inline-block;
                line-height: 116px;
                padding-bottom: 4px;

                &:hover {
                    color: blue;
                    border-bottom: 4px solid blue;
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

        // test
        // background-color: darkred;
    }
</style>