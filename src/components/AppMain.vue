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
        
        .container {
            width: 1200px;
            height: 7rem;
            @include flex-centered()
        }
    }

</style>