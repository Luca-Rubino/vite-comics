<script>
export default {
    data() {
        return {
            dcComicsLink: [
                {
                    id: 1,
                    title: "Characters",
                    link: "#"
                },

                {
                    id: 2,
                    title: "Comics",
                    link: "#"
                },

                {
                    id: 3,
                    title: "Movies",
                    link: "#"
                },

                {
                    id: 4,
                    title: "TV",
                    link: "#"
                },

                {
                    id: 5,
                    title: "Games",
                    link: "#"
                },

                {
                    id: 6,
                    title: "Videos",
                    link: "#"
                },

                {
                    id: 7,
                    title: "News",
                    link: "#"
                }
            ],

            shop: [
                {
                    id: 1,
                    title: "Shop DC",
                    link: "#"
                },
                
                {
                    id: 2,
                    title: "Shop DC Collectibles",
                    link: "#"
                },
            ],

            dc: [
                {
                    id: 1,
                    title: "Term Of Use",
                    link: "#"
                },

                {
                    id: 2,
                    title: "Privacy Policy (New)",
                    link: "#"
                },

                {
                    id: 3,
                    title: "Ad Choices",
                    link: "#"
                },

                {
                    id: 4,
                    title: "Advertising",
                    link: "#"
                },

                {
                    id: 5,
                    title: "Jobs",
                    link: "#"
                },

                {
                    id: 6,
                    title: "Subscription",
                    link: "#"
                },

                {
                    id: 7,
                    title: "Tallene Workshop",
                    link: "#"
                },

                {
                    id: 8,
                    title: "CPSC Certificates",
                    link: "#"
                },

                {
                    id: 9,
                    title: "Ratings",
                    link: "#"
                },

                {
                    id: 10,
                    title: "Shop Help",
                    link: "#"
                },

                {
                    id: 11,
                    title: "Contact Us",
                    link: "#"
                }
            ],

            sites: [
                {
                    id: 1,
                    title: "DC", 
                    link: "#"
                },

                {
                    id: 2,
                    title: "MAD Magazine", 
                    link: "#"
                },

                {
                    id: 3,
                    title: "DC Kids", 
                    link: "#"
                },

                {
                    id: 4,
                    title: "DC Universe", 
                    link: "#"
                },

                {
                    id: 5,
                    title: "DC Power Visa", 
                    link: "#"
                }

            ],

            socials: [
                {
                    id:1,
                    social: 'facebook',
                    url: './src/assets/img/footer-facebook.png'
                },

                {
                    id:2,
                    social: 'twitter',
                    url: './src/assets/img/footer-twitter.png'
                },

                {
                    id:3,
                    social: 'youtube',
                    url: './src/assets/img/footer-youtube.png'
                },

                {
                    id:4,
                    social: 'pinterest',
                    url: './src/assets/img/footer-pinterest.png'
                },

                {
                    id:5,
                    social: 'periscope',
                    url: './src/assets/img/footer-periscope.png'
                }
            ]
        }
    },
}
</script>

<template>

    <footer>
        <div class="container-link">
            <section class="link">
                <nav>
                    <h2>dc comics</h2>
                    <ul>
                        <li v-for="(title, index) in dcComicsLink">
                            <a :href="title.link">{{ title.title }}</a>
                        </li>
                    </ul>
                    <h2>shop</h2>
                    <ul>
                        <li v-for="title in shop">
                            <a :href="title.link">{{ title.title }}</a>
                        </li>
                    </ul>
                </nav>

                <nav>
                    <h2>dc</h2>
                    <ul>
                        <li v-for="title in dc">
                            <a :href="title.link">{{ title.title }}</a>
                        </li>
                    </ul>
                </nav>

                <nav>
                    <h2>dc</h2>
                    <ul>
                        <li v-for="title in sites">
                            <a :href="title.link">{{ title.title }}</a>
                        </li>
                    </ul>
                </nav>
                
            </section>
        
            <section class="logo">
                <img src="../assets/img/dc-logo-bg.png" alt="dc-logo-bg">
            </section>
        </div>
    </footer>



</template>

<style lang="scss" scoped>
    @use '../../styles/partials/appFooter.scss' as *;
</style>
