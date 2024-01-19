<script>
    import SingleProduct from './SingleProduct.vue';


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
                ],

                comics: [
  {
      "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
      "price": "$19.99",
      "series": "Action Comics",
      "type": "comic book",
  },
  {
      "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
      "price": "$3.99",
      "series": "American Vampire 1976",
      "type": "comic book",
  },
  {
      "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
      "price": "$16.99",
      "series": "Aquaman",
      "type": "graphic novel",
  },
  {
      "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
      "price": "$2.99",
      "series": "Batgirl",
      "type": "comic book",
  },
  {
      "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
      "price": "$3.99",
      "series": "Batman",
      "type": "comic book",
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
      "price": "$2.99",
      "series": "Batman Beyond",
      "type": "comic book",
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
      "price": "$3.99",
      "series": "Batman/Superman",
      "type": "comic book",
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
      "price": "$4.99",
      "series": "Batman/Superman Annual",
      "type": "comic book",
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
      "price": "$5.99",
      "series": "Batman: The Joker War Zone",
      "type": "comic book",
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
      "price": "$6.99",
      "series": "Batman: Three Jokers",
      "type": "comic book",
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
      "price": "$4.99",
      "series": "Batman: White Knight Presents: Harley Quinn",
      "type": "comic book",
  },
  {
      "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
      "price": "$16.99",
      "series": "Catwoman",
      "type": "graphic novel",
  },
]
            };
        },
        components: {
           SingleProduct
        }
    }
</script>

<template>
    <main>
        <section id="Content-container">
            <div id="jumbotron">        
            </div>
            <div class="series-container">
                <div class="container">
                    <div class="h1-container">
                        <h1>
                            CURRENT SERIES
                        </h1>
                    </div>

                    <div class="products-container" >
                        <SingleProduct v-for="(comic, i) in comics" :key="i" :product="comic"/>                        
                    </div>
                </div>
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

.products-container {
    display: flex;
    flex-wrap: wrap;
    padding: 50px 0;
}
</style>
