<script>
export default {
    data() {
        return {
            navbarLinks: [
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
                    title: "Collectibles",
                    active: false
                },
                {
                    id: 7,
                    title: "Videos",
                    active: false
                },
                {
                    id: 8,
                    title: "Fans",
                    active: false
                },
                {
                    id: 9,
                    title: "News",
                    active: false
                },
                {
                    id: 10,
                    title: "Shop",
                    active: false
                },
            ]
        };
    }
};
</script>

<template>
    <header>
        <div class="container">
            <section class="logo">
                <img src="../assets/img/dc-logo.png" alt="header-logo">
            </section>
            <nav class="navbar">
                <ul>
                    <li v-for="link in navbarLinks" key="id">
                        {{ link.title.toUpperCase() }}
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style scoped lang="scss">
    header {
        width: 100%;
        
        .container {
            margin: 0 auto;
            width: 1200px;
            height: 5rem;
            display: flex;
            align-items: center;
            justify-content: space-between;

            .logo {
                display: flex;
                align-items: center;
                padding: 1rem 0;
                img {
                    width: 60%;
                }
            }
        }
    }

    ul {
        display: flex;

        li {
            margin-right: 1rem;
            font-weight: bold;
        }
    }
</style>