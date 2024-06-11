<script>
import AppMainContent from "./AppMainContent.vue";


export default {
    components: {
        AppMainContent,
    },

    data() {
        return {
    
        };
    }
};
</script>

<template>
    <main>
        <div class="jumbotron">

        </div>
        <div class="container">
            <div class="content-label">
                <h2>
                    Current Series
                </h2>
            </div>
            <AppMainContent />
        </div>
    </main>
</template>

<style scoped lang="scss">
@use "../styles/partials/mixins" as *;
@use "../styles/partials/variables" as *;

    main {
        background-color: #1c1c1c;
        color: white;

        .jumbotron {
            height: 15rem;
            background-image: url(../assets/img/jumbotron.jpg);
            background-repeat: no-repeat;
            background-size: cover;
        }
        
        .container {
            position: relative;
            width: 1200px;
            @include flex-centered();
            flex-direction: column;
            align-items: start;

            .content-label {
                @include flex-centered();
                position: relative;
                height: 50px;
                left: 0;
                top: -25px;
                background-color: $footer-blue;
                text-transform: uppercase;
                padding: .5rem 1rem;
            }
        }
    }

</style>