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
    </header>
</template>

<style scoped>

</style>