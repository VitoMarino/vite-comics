<script>
export default{
    data() {
        return {
        }    
    }
}
</script>

<template>
<main>
    <section>
        <p>
        --> Content goes here <--
        </p>
    </section>
</main>
</template>

<style lang="scss" scoped>
    @use '../styles/parziali/variabili'  as *;
    @use '../styles/parziali/mixins' as*;
    
    section{
        width: 100vw;
        height: 5rem;
        background-color: $bg_color_black;
        color: white;
        @include my_d_flex_two;
    }
</style>