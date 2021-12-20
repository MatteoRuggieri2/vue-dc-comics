<template>
    <section>
        <div class="container">

            <!-- Link list -->
            <div class="link-list">
                <div class="list-container">
                    <h3>title list</h3>
                    <ul>
                        <li>test</li>
                        <li>test</li>
                        <li>test</li>
                        <li>test</li>
                        <li>test</li>
                        <li>test</li>
                        <li>test</li>
                    </ul>

                    <h3>title list</h3>
                    <ul>
                        <li>test</li>
                        <li>test</li>
                    </ul>
                </div>

                <div class="list-container">
                    <h3>title list</h3>
                    <ul>
                        <li>test</li>
                        <li>test</li>
                        <li>test</li>
                        <li>test</li>
                        <li>test</li>
                        <li>test</li>
                        <li>test</li>
                        <li>test</li>
                        <li>test</li>
                        <li>test</li>
                        <li>test</li>
                    </ul>
                </div>

                <div class="list-container">
                    <h3>title list</h3>
                    <ul>
                        <li>test</li>
                        <li>test</li>
                        <li>test</li>
                        <li>test</li>
                        <li>test</li>
                    </ul>
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
    name: "FooterLinkList"
}
</script>

<style lang="scss" scoped>

    section {
        padding: 50px 0;
        color: white;
        background-image: url(../assets/img/footer-bg.jpg);
        overflow: hidden;

        .container {
            
            position: relative;

            .link-list{
                display: flex;

                // test
                background-color: yellowgreen;

                .list-container {
                    margin: 0 20px;

                    ul {
                        margin-bottom: 20px;
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