<script>
export default {
    data() {
        return {
        
        };
    },

    props: {
        article: {
            type: Object,
            required: true,
        },
    }
};
</script>

<template>
    <article class="comics-item">
        <img :src="article.thumb" :alt="article.series + '-img'">
        <p>
            {{ article.series }}
        </p>
    </article>
</template>

<style scoped lang="scss">
    article{
        height: 100%;
        img {
            width: 100%;
            aspect-ratio: 1/1;
            object-fit: cover;
            object-position: top;
            margin-bottom: .5rem;
        }
    }
</style>