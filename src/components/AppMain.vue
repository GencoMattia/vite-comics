<script>
export default {
    data() {
        return {
    
        };
    }
};
</script>

<template>
    <main>
        <div class="container">
            <section class="content">
                <h2>
                    --> Content goes here <--
                </h2>
            </section>
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