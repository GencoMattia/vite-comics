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
            <AppMainContent />
        </div>
    </main>
</template>

<style scoped lang="scss">
@use "../styles/partials/mixins" as *;

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
            width: 1200px;
            // height: 7rem;
            @include flex-centered()
        }
    }

</style>