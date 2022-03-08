<template>
    <div class="banner">
        <div class="container-s">
            <ul>
                <li class="item">
                    <a href="#">
                        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                        Digital Comics
                    </a>    
                </li>  
                <li class="item">
                    <a href="#">
                        <img src="../assets/img/buy-comics-merchandise.png" alt="">
                        DC Merchandise
                    </a>
                </li>
                <li class="item">
                    <a href="#">
                        <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                        Subscription
                    </a>
                </li>
                <li class="item">
                    <a href="#">
                        <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                        Comic Shop Location
                    </a>
                </li>
                <li class="item">
                    <a href="#">
                        <img class="svg" src="../assets/img/buy-dc-power-visa.svg" alt="">
                        DC Power Visa
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: 'PageBanner'
}
</script>

<style lang="scss" scoped>
.banner {
    background-color: var(--app-blue);
    padding: 50px 0;

    .container-s {
        max-width: 1024px;
        margin: 0 auto;

        ul {
            display: flex;
            list-style: none;
            gap: 15px;

            .item {
                display: flex;
                align-items: center;
                gap: 10px;
                width: 20%;

                a {
                    color: white;
                    text-decoration: none;
                    display: contents;
                    text-transform: uppercase;
                    font-size: 0.7rem;
                    
                    img {
                    height: 60px;

                    &.svg {
                        height: 40px;
                    }
                    
                }
                }
                
            }
        }
    }
}
</style>