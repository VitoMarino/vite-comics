<script>
    export default{
    data() {
        return {
        }    
    },
    props: {
        singleCard: {
            type: Object,
            required: true,
        }
    }
}
</script>

<template>
        <article>
            <img :src="singleCard.thumb" :alt="singleCard.type">
        <h4>
            {{ singleCard.series }}
        </h4>
        <p>
            {{ singleCard.price }}
        </p>
        </article>
</template>

<style lang="scss" scoped>
    article {
            width: calc((100% / 6) - 2rem);
            font-size: 10px;
            margin: 1rem;

            img {
                width: 100%;
            }
        }
</style>