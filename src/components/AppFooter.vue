<script>
export default {
    data() {
        return {

        }
    }
}
</script>

<template>
    <Footer>
        <div class="container">
            <section class="logo-links">
                <nav class="site-links">

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
</style>