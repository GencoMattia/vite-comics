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
        }
    }
}
</script>

<template>
    <Footer>
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
            <nav class="social-links">

            </nav>
        </div>
    </Footer>
</template>

<style scoped>
    footer {
        background-image: url(../assets/img/footer-bg.jpg);
        background-repeat: no-repeat;
        background-size: cover;
    }

    .logo-links {
        display: flex;
        height: 15rem;
        width: 50%;
    }

    .container{
        display: flex;
        flex-direction: column;

        .footer-logo {
            width: 50%;
        }
    }

    h2 {
        text-transform: uppercase;
    }
</style>