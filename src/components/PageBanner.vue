<template>
    <div class="banner">
        <div class="container-s">
            <ul>
                <li v-for="(item, i) in bannerItems" :key="i" class="item">
                    <a href="#">
                        <img :src="require(`../assets/img/${item.img}`)" alt="">
                        {{ item.name }}
                    </a>    
                </li>  
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: 'PageBanner',
    data() {
        return {
            bannerItems: [
                {
                    name: 'Digital Comics',
                    img: 'buy-comics-digital-comics.png'
                },
                {
                    name: 'DC Merchandise',
                    img: 'buy-comics-merchandise.png'
                },
                {
                    name: 'Subscription',
                    img: 'buy-comics-subscriptions.png'
                },
                {
                    name: 'Comic Shop Location',
                    img: 'buy-comics-shop-locator.png'
                },
                {
                    name: 'DC Power Visa',
                    img: 'buy-dc-power-visa.svg'
                },
            ]
        }
    }
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

                    &:last-child {
                        height: 40px;
                    }
                    
                    
                }
                }
                
            }
        }
    }
}
</style>