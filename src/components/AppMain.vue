<script>
import Comics from '../components/Comics.vue';
import CardDcComics from '../components/CardDcComics.vue';


export default {
        components: {
            Comics,
            CardDcComics
        },

    data() {
        return {
            comicSeries: [
                {
                    "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ]
        }
    },
}

</script>

<template>

    <main>
        <section class="container">
            <article>
                <h1> Current Series</h1>
                <div class="comics">
                    <CardDcComics v-for="(comic, index) in comicSeries" :key="index" :singleComic="comic" />
                </div>
                <button>Load More</button>
            </article>
        </section>

        <!-- 
        <section class="content">

            <p>Content goes here</p>
            
        </section>
        -->

        <Comics/>
    </main>

</template>

<style lang="scss" scoped>
@use '../../styles/general.scss' as *;
@use '../../styles/partials/variable.sass' as *;
@use '../../styles/partials/mixin.sass' as *;

section.content {
  background-color: black;
  color: white;
  padding: 3rem 13rem;
  font-size: 1.5rem;
  width: 100%;
}

section.container{
    background-color: #1c1c1c;
    color: white;

    h1 {
        margin: 0 19rem;
        position: relative;
        bottom: 1.2rem;
        text-transform: uppercase;
        background-color: #0282f9;
        width: 9.9rem;
        padding: 0.5rem;
        font-size: 1.1rem;
    }

    div.comics {
        display: flex;
        flex-wrap: wrap;
        margin: 0 19rem;
    }

    button{
        margin-left: 54rem;
        background-color: #0282f9;
        border: 0;
        color: white;
        font-size: 1rem;
        font-weight: 900;
        font-family: "Roboto", sans-serif;
        padding: .5rem 4rem;
        margin-bottom: 1rem;
    }
}
</style>