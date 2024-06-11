<script>
export default {
    data() {
        return {
            headerLink: [
                {
                  id: 1,
                  title: "characters",
                  active: false,
                  link: "#"
                },

                {
                  id: 2,
                  title: "comics",
                  active: true,
                  link: "#" 
                },

                { 
                  id: 3,
                  title: "movies",
                  active: false,
                  link: "#"
                },

                {
                  id: 4,
                  title: "tv",
                  active: false,
                  link: "#"
                },

                {
                  id: 5,
                  title: "games",
                  active: false,
                  link: "#"
                },

                {
                  id: 6,
                  title: "collectibles",
                  active: false,
                  link: "#"
                },

                {
                  id: 7,
                  title: "videos",
                  active: false, 
                  link: "#"
                },

                {
                  id: 8,
                  title: "fan",
                  active: false,
                  link: "#" },
                {
                  id: 9,
                  title: "news",
                  active: false,
                  link: "#"
                },

                {
                  id: 10,
                  title: "shop",
                  active: false,
                  link: "#"
                }
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
</header>

<main>
    <div class="content">

        <p>-->Content goes here<--</p>
        
    </div>
</main>

</template>

<style lang="scss" scoped>

header > div {
  display: flex;
  width: 100%;
  justify-content: space-evenly;
}

section.list-title {
  display: flex;
  align-items: center;
}

ul{
  display: flex;
}

li{
  margin-right: 1rem;
}

div.content{
  background-color: black;
  color: white;
  padding: 2rem 13rem;
  font-size: 1.5rem;
}

</style>