<script>
import ComicCardApp from './card/ComicCardApp.vue'

    export default {
        name: "ContentApp",
        components: {
            ComicCardApp,
        },

        data() {
            return {
                seriesList: [
                    {
                        thumb: "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                        price: "$19.99",
                        series: "Action Comics",
                        type: "comic book",
                    },
                    {
                        thumb: "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                        price: "$3.99",
                        series: "American Vampire 1976",
                        type: "comic book",
                    },
                    {
                        thumb: "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                        price: "$16.99",
                        series: "Aquaman",
                        type: "graphic novel",
                    },
                    {
                        thumb: "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                        price: "$2.99",
                        series: "Batgirl",
                        type: "comic book",
                    },
                    {
                        thumb: "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                        price: "$3.99",
                        series: "Batman",
                        type: "comic book",
                    },
                    {
                        thumb: "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                        price: "$2.99",
                        series: "Batman Beyond",
                        type: "comic book",
                    },
                    {
                        thumb: "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                        price: "$3.99",
                        series: "Batman/Superman",
                        type: "comic book",
                    },
                    {
                        thumb: "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                        price: "$4.99",
                        series: "Batman/Superman Annual",
                        type: "comic book",
                    },
                    {
                        thumb: "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                        price: "$5.99",
                        series: "Batman: The Joker War Zone",
                        type: "comic book",
                    },
                    {
                        thumb: "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                        price: "$6.99",
                        series: "Batman: Three Jokers",
                        type: "comic book",
                    },
                    {
                        thumb: "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                        price: "$4.99",
                        series: "Batman: White Knight Presents: Harley Quinn",
                        type: "comic book",
                    },
                    {
                        thumb: "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                        price: "$16.99",
                        series: "Catwoman",
                        type: "graphic novel",
                    },
                ]
            }
        }
    };

</script>

<template>
    <main>
        <div>
            <img class="jumbo" src="/src/assets/jumbotron.jpg" alt="">
        </div>


        <div class="container card-grid">
            <button id="current-series-button">CURRENT SERIES</button>

            <ComicCardApp v-for="(comic, index) in seriesList" :key="index" :item="comic"/>
        </div>

        <div class="container">
            <button>LOAD MORE</button>
        </div>
    </main>
</template>

<style lang="scss" scoped>
@use '/src/style/partials/variables' as *;

.jumbo {
    max-width: 100%;
}

main {
    background-color: black;
}

.card-grid {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
    gap: 10px;
    position: relative;
}

button {
    width: 15%;
    background-color: $primary;
    display: block;
    margin: 0 auto;
    padding: 10px;
    font-size: 1.1rem;
    font-weight: bold;
    color: white;
    border: none;
    cursor:pointer;
}

.container {
    padding-bottom: 20px;
}

#current-series-button {
    width: 15%;
    background-color: $primary;
    display: block;
    padding: 10px;
    font-size: 1.2rem;
    color: white;
    border: none;
    cursor:pointer;
    position: absolute;
    top: -30px;
    left: 12px;
    font-weight: bold;
}

</style>