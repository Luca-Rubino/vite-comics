<script>
export default {
    data() {
        return {
            headerLink: [
                { id: 1, title: "characters", active: false, link: "#" },

                { id: 2, title: "comics", active: true, link: "#" },

                { id: 3, title: "movies", active: false, link: "#" },

                {  id: 4, title: "tv", active: false, link: "#" },

                { id: 5, title: "games", active: false, link: "#" },

                { id: 6, title: "collectibles", active: false, link: "#" },

                { id: 7, title: "videos", active: false, link: "#" },

                { id: 8, title: "fan", active: false, link: "#" },

                { id: 9, title: "news", active: false, link: "#" },

                { id: 10, title: "shop", active: false, link: "#"}
            ]
        }
    },
}
</script>

<template>

    
<header>

    <div class="container">

        <section class="image">
            <img src="../assets/img/dc-logo.png" alt="dc-logo">
        </section>

        <section class="list-title">

            <ul>
                <li v-for="(title,index) in headerLink" :key="title.id">
                    {{ title.title }}
                </li>
            </ul>

        </section>
        
    </div>

    <div class="jumbotron"></div>

</header>

</template>

<style lang="scss" scoped>
@use '../../styles/partials/appHeader.scss' as *;
</style>