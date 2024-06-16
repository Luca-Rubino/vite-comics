<script>

export default {

    data() {
        return {
            comics: [
                { immagine: '../../src/assets/img/buy-comics-digital-comics.png', titolo: 'digital comics' },

                { immagine: '../../src/assets/img/buy-comics-merchandise.png', titolo: 'merchandise' },

                { immagine: '../../src/assets/img/buy-comics-subscriptions.png', titolo: 'subscription' },

                { immagine: '.../../src/assets/img/buy-comics-shop-locator.png', titolo: 'comics shop locator' },

                { immagine: '../../src/assets/buy-dc-power-visa.svg', titolo: 'dc power visa' }
            ],

            index: 0
        }
    },
}

</script>

<template>
    <section>
        <ul>
            <li v-for="(comics, index) in comics">
                <img :src="comics.immagine" :alt="comics.titolo">
                <p>{{ comics.titolo  }}</p>
            </li>
        </ul>
    </section>
</template>

<style lang="scss" scoped>
@use '../../styles/general.scss' as *;
@use '../../styles/partials/variable.sass' as *;
@use '../../styles/partials/mixin.sass' as *;

section {
    background-color: #0282f9;
    color: white;
    padding: 2rem 0;

    ul {
        display: flex;
        margin-left: 22rem;
        font-weight: 300;
        font-size: 1rem;

        li {
            display: flex;
            align-items: center;

            img {
                width: 3rem;
                margin-right: .5rem;
            }

            p {
                margin-right: 5rem;
            }
        }
    }
}
</style>