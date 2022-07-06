<template>
    <section>
        <div class="container">
            <ul>
                <!-- Links -->
                <li v-for="(link, index) in menuLinks" :key="index">
                    <a :href="link.url">

                        <!-- link Image -->
                        <div class="buy-img">
                            <img :src="link.image" :alt="link.text">
                        </div>
                        
                        <!-- link Info -->
                        <div class="text">
                            {{ link.text }}
                        </div>    
                    </a>
                </li>
            </ul>
        </div>
    </section>
</template>

<script>
    export default {
        name: "SectionBuyList",
        data() {
            return {
                menuLinks: [
                    {
                        text: 'DIGITAL COMICS',
                        image: require('../assets/img/buy-comics-digital-comics.png'),
                        url: '#',
                    },
                    {
                        text: 'DC MERCHANDISE',
                        image: require('../assets/img/buy-comics-merchandise.png'),
                        url: '#',
                    },
                    {
                        text: 'SUBSCRIPTION',
                        image: require('../assets/img/buy-comics-subscriptions.png'),
                        url: '#',
                    },
                    {
                        text: 'COMIC SHOP LOCATOR',
                        image: require('../assets/img/buy-comics-shop-locator.png'),
                        url: '#',
                    },
                    {
                        text: 'DC POWER VISA',
                        image: require('../assets/img/buy-dc-power-visa.svg'),
                        url: '#',
                    },
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
@import '../style/variables';
section {
    display: flex;
    justify-content: center;
    background-color: $brand_main_color;
    padding: 40px 0;
    
    .buy-img {
        width: 40px;
    }
    img {
        display: inline-block;
    }

    ul {
        display: flex;
        justify-content: center;
        align-items: center;
    }

    li {
        padding: 0px 25px ;
        
        a {
            text-decoration: none;
            color: white;
            display: flex;
            align-items: center;
            cursor: pointer;
            .text {
                padding-left: 10px;
                font-size: 14px;
            }
        }
    }
}
</style>