<template>
    <header>
        <div class="container">
            <div class="main-header">
                <!-- Header logo -->
                <div class="logo">
                    <img src="../assets/img/dc-logo.png" alt="DC logo">
                </div>
                
                <!-- Header Nav -->
                <nav>
                <ul class="menu">
                    <li v-for="(link, index) in menuLinks" :key="index" :class="{ 'current': link.current }">
                        <a :href="link.url" :class="{ 'current': link.current }">{{ link.text }}</a>
                    </li>
                </ul>
                </nav>
            </div>

        </div>
    </header>
</template>

<script>
export default {
    name: "PageHeader",
    data() {
        return {
            menuLinks: [
                {
                    text: 'Characters',
                    url: '#',
                    current: false
                },
                {
                    text: 'Comics',
                    url: '#',
                    current: true
                },  
                {
                    text: 'Movies',
                    url: '#',
                    current: false
                },
                {
                    text: 'Tv',
                    url: '#',
                    current: false
                },
                {
                    text: 'Games',
                    url: '#',
                    current: false
                },
                {
                    text: 'Collectibles',
                    url: '#',
                    current: false
                },
                {
                    text: 'Videos',
                    url: '#',
                    current: false
                },
                {
                    text: 'Fans',
                    url: '#',
                    current: false  
                },
                {
                    text: 'News',
                    url: '#',
                    current: false
                },
                {
                    text: 'Shop',
                    url: '#',
                    current: false
                },
            ]
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../style/variables";

header {
    background-color: white;
    width: 100%;
    height: 100px;
    position: fixed;
    top: 0;
    z-index: 1000;
    .main-header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        
        // Logo
        .logo {
            img {
                width: 75px;
                display: inline-block;
            }
        }

        // Nav
        .menu {
        margin: 30px 0;
        display: flex;
        justify-content: center;
        
            li {
                padding: 10px;
                text-decoration: none;
                cursor: pointer;

                &.current {
                    border-bottom: 1px solid $brand_main_color;
                    border-bottom-width: 5px;  
                }

                a {
                    color: black;
                    font-size: 14px;
                    font-weight: 700;
                    text-transform: uppercase;

                &.current {
                    color: $brand_main_color;
                }
                }

            }
        }
    }
}

</style>