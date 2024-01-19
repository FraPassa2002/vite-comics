<script>
    // import SingleProduct from './SingleProduct.vue';


    export default {
        data() {
            return {
                options: [
                    {
                        name: 'DIGITAL COMICS',
                        image: '../../public/img/buy-comics-digital-comics.png'
                    },
                    {
                        name: 'DC MERCHANDISE',
                        image: '../../public/img/buy-comics-merchandise.png'
                    },
                    {
                        name: 'SUBSCRIPTION',
                        image: '../../public/img/buy-comics-subscriptions.png'
                    },
                    {
                        name: 'COMIC SHOP LOCATOR',
                        image: '../../public/img/buy-comics-shop-locator.png'
                    },
                    {
                        name: 'DC POWER VISA',
                        image: '../../public/img/buy-dc-power-visa.svg'
                    },
                ]
            };
        },
        //  components: {
        //     SingleProduct
        //  }
    }
</script>

<template>
    <main>
        <section id="Content-container">
            <div class="container">
                <h1>
                    <a href="#">
                    Content goes here 
                    </a>
                </h1>
            </div>
        </section>
        <section id="market-container">
            <div class="container">
                <ul>
                    <li v-for="(option, i) in options" key="i">
                        <a href="#">
                            <img :src="option.image" :alt="option.name">
                            <p>
                                {{ option.name }}
                            </p>
                        </a>
                    </li>
                </ul>
            </div>
        </section>
        <section id="credits-container">
            <div class="container">
                <div class="cols">
                    <div>
                        <h4>
                            DC COMICS
                        </h4>
                        <ul>
                            <li v-for="i in 7" :key="i">
                                <a href="#">
                                    Link
                                </a>
                            </li>
                        </ul>
                    </div>

                    <div>
                        <h4>
                            DC
                        </h4>
                        <ul>
                            <li v-for="i in 3" :key="i">
                                <a href="#">
                                    Link
                                </a>
                            </li>
                        </ul>
                    </div>
                    <div>
                        <h4>
                            SITES
                        </h4>
                        <ul>
                            <li v-for="i in 5" :key="i">
                                <a href="#">
                                    Link
                                </a>
                            </li>
                        </ul>
                    </div>
                    <div>
                        <h4>
                            SHOP
                        </h4>
                        <ul>
                            <li v-for="i in 6" :key="i">
                                <a href="#">
                                    Link
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>

                <div class="image-container">
                </div>
            </div>
        </section>
    </main>
</template>

<style lang="scss" scoped>
    
</style>
