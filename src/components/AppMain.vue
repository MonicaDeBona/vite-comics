<script>
    export default {
        name: 'AppMain',
        data() {
            return {
                blueLogos: [
                    {
                        text: 'DIGITAL COMICS',
                        path: "buy-comics-digital-comics.png"
                    },
                    {
                        text: 'DC MERCHANDISE',
                        path: "buy-comics-merchandise.png"
                    },
                    {
                        text: 'SUBSCRIPTION',
                        path: "buy-comics-subscriptions.png"
                    },
                    {
                        text: 'COMIC SHOP LOCATOR',
                        path: 'buy-comics-shop-locator.png'
                    },
                    {
                        text: 'DC POWER VISA',
                        path: "buy-dc-power-visa.svg"
                    }
                ],
            }
        },

        methods: {
            getImagePath: function (img) {
                return new URL(`../assets/imgs/${img}`, import.meta.url).href;   
            }
        }
}
</script>

<template>
    <section class="main-content">
        <div class="my-container">
            <h2>> Content goes here &lt;</h2>
        </div>
    </section>
    <section class="blue-banner">
        <div class="my-container">
            <ul>
                <li v-for="item in blueLogos">
                    <img :src="getImagePath(item.path)" :alt="item.text">
                    <h5>{{ item.text }}</h5>
                </li>
            </ul>
        </div>
    </section>
</template>



<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

    .main-content {
        background-color: $main-color;
    }

    .blue-banner {
        background-color: $blue-color;
        padding: 3rem;
        color: $white-color;
    }

    ul {
        display: flex;
        justify-content: space-around;
        list-style-type: none;

        li {
            display: flex;
            align-items: center;

            img {
                height: 50px;
                padding-right: 1rem;
            }
        }
    }

</style>