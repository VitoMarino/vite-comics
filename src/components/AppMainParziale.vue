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
    <main>
        <img :src="singleCard.thumb" :alt="singleCard.type">
        <h4>
            {{ singleCard.series }}
        </h4>
        <p>
            {{ singleCard.price }}
        </p>
    </main>
</template>

<style lang="scss" scoped>
    article {
            width: calc((100% / 6) - 4rem);
            font-size: 10px;
            margin: 2rem;

            img {
                width: 100%;
            }
        }
</style>