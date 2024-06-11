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
    <section class="jumbotron">
        
    </section>
</main>
</template>

<style lang="scss" scoped>
    @use '../styles/parziali/variabili'  as *;
    @use '../styles/parziali/mixins' as*;
    
    section.jumbotron{
        width: 100vw;
        height: 18rem;
        background-image: url(/img/jumbotron.jpg);
        background-size: cover;
    }
</style>