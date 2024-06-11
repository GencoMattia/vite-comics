<script>
export default {
    data() {
        return {
            DcComicsList: [
                {
                    id: 1,
                    title: "Characters",
                    active: false
                },
                {
                    id: 2,
                    title: "Comics",
                    active: true
                },
                {
                    id: 3,
                    title: "Movies",
                    active: false
                },
                {
                    id: 4,
                    title: "Tv",
                    active: false
                },
                {
                    id: 5,
                    title: "Games",
                    active: false
                },
                {
                    id: 6,
                    title: "Videos",
                    active: false
                },
                {
                    id: 7,
                    title: "News",
                    active: false
                },
            ],

            ShopList: [
                {
                    id: 1,
                    title: "Shop DC",
                    active: false
                },
                {
                    id: 2,
                    title: "Shop DC Collectibles",
                    active: false
                },
            ],

            DcList: [
                {
                    id: 1,
                    title: "Terms Of Use",
                    active: false
                },
                {
                    id: 2,
                    title: "Privacy Policy (New)",
                    active: true
                },
                {
                    id: 3,
                    title: "Ad Choices",
                    active: false
                },
                {
                    id: 4,
                    title: "Advertising",
                    active: false
                },
                {
                    id: 5,
                    title: "Jobs",
                    active: false
                },
                {
                    id: 6,
                    title: "Subscriptions",
                    active: false
                },
                {
                    id: 7,
                    title: "Talent Workshops",
                    active: false
                },
                {
                    id: 8,
                    title: "CPSC Certificates",
                    active: false
                },
                {
                    id: 9,
                    title: "Ratings",
                    active: false
                },
                {
                    id: 10,
                    title: "Shop Help",
                    active: false
                },
                {
                    id: 11,
                    title: "Contact Us",
                    active: false
                },
            ],

            SiteList: [
                {
                    id: 1,
                    title: "DC",
                    active: false
                },
                {
                    id: 2,
                    title: "MAD Magazines",
                    active: false
                },
                {
                    id: 3,
                    title: "DC Kids",
                    active: false
                },
                {
                    id: 4,
                    title: "DC Universe",
                    active: false
                },
                {
                    id: 5,
                    title: "DC Power Visa",
                    active: false
                },
            ],

            SocialList: [
                {
                    id: 1,
                    name: "Facebook",
                    icon: "footer-facebook.png"
                },
                {
                    id: 2,
                    name: "Twitter",
                    icon: "footer-twitter.png"
                },
                {
                    id: 3,
                    name: "YouTube",
                    icon: "footer-youtube.png"
                },
                {
                    id: 4,
                    name: "Pinterest",
                    icon: "footer-pinterest.png"
                },
                {
                    id: 5,
                    name: "Periscope",
                    icon: "footer-periscope.png"
                },
            ],
        }
    },

    methods: {
        getImagePath: function(img) {
            return new URL(`../assets/img/${img}`, import.meta.url).href;
        }
    },
}
</script>

<template>
    <footer>
        <div class="container">
            <section class="logo-links">
                <nav class="site-links">
                    <div class="dc-comics-list">
                        <h2>
                            DC Comics
                        </h2>
                        <ul>
                            <li v-for="link in DcComicsList" key="id">
                                {{ link.title }}
                            </li>
                        </ul>
                    </div>
                    <div class="dc-comics-list">
                        <h2>
                            Shop
                        </h2>
                        <ul>
                            <li v-for="link in ShopList" key="id">
                                {{ link.title }}
                            </li>
                        </ul>
                    </div>
                    <div class="dc-comics-list">
                        <h2>
                            DC
                        </h2>
                        <ul>
                            <li v-for="link in DcList" key="id">
                                {{ link.title }}
                            </li>
                        </ul>
                    </div>
                    <div class="dc-comics-list">
                        <h2>
                            Sites
                        </h2>
                        <ul>
                            <li v-for="link in SiteList" key="id">
                                {{ link.title }}
                            </li>
                        </ul>
                    </div>
                </nav>
                <div class="footer-logo">
                    <img src="../assets/img/dc-logo-bg.png" alt="footer-logo">
                </div>
            </section>
        </div>
        <section class="footer-socials">
            <div class="container">
                <nav class="social-links">
                    <button class="sign-up">
                        Sign Up Now!
                    </button>
                    <div class="socials-list">
                        <h2>
                            Follow Us
                        </h2>
                        <ul>
                            <li v-for="link in SocialList" key="id">
                                <img :src="getImagePath(link.icon)" :alt="link.name + '-img'">
                            </li>
                        </ul>
                    </div>
                </nav>
            </div>
        </section>
    </footer>
</template>

<style scoped lang="scss">
@use "../styles/partials/variables" as *;

    footer {
        background-image: url(../assets/img/footer-bg.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        overflow: hidden;
    }

    .container{
        display: flex;
        flex-direction: column;

        .logo-links {
            width: 100%;
            display: flex;
            justify-content: space-between;
            height: 15rem;
            color: #959595;
            
            .site-links {
                width: 50%;
                display: flex;
                flex-direction: column;
                flex-wrap: wrap;
            }
    
            h2 {
                color: white;
                text-transform: uppercase;
            }
    
            .footer-logo {
                display: flex;
                justify-content: end;
                align-items: center;
    
                img {
                    height: 120%;
                }
            }
        }

        .footer-logo {
            width: 50%;
            overflow: hidden;
        }
    }

    .footer-socials {
        width: 100%;
        background-color: #303030;

        .container {
            height: 4rem;

            .social-links {
                height: 100%;
                display: flex;
                justify-content: space-between;
                align-items: center;

                button {
                    background-color: transparent;
                    border: $footer-blue solid 2px;
                    color: white;
                    text-transform: uppercase;
                    padding: .5rem 1rem;

                    &:hover {
                        background-color: rgba($color: #ffffff, $alpha: .1);
                    }
                }

                .socials-list {
                    display: flex;
                    color: #959595;

                    h2 {
                        color: $footer-blue;
                        text-transform: uppercase;
                    }

                    ul {
                        display: flex;
                    }
                }
            }
        }
    }


</style>