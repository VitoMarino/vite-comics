<script>
export default{
    data() {
        return {
            headerLink: [
            {
                id: 1,
                title: "Characters",
                active: false,
                url: '#'
            },
            {
                id: 2,
                title: "Comics",
                active: false,
                url: '#'
            },
            {
                id: 3,
                title: "Movies",
                active: false,
                url: '#'
            },
            {
                id: 4,
                title: "TV",
                active: false,
                url: '#'
            },
            {
                id: 5,
                title: "Games",
                active: false,
                url: '#'
            },
            {
                id: 6,
                title: "Collectibles",
                active: false,
                url: '#'
            },
            {
                id: 7,
                title: "Videos",
                active: false,
                url: '#'
            },
            {
                id: 8,
                title: "Fans",
                active: false,
                url: '#'
            },
            {
                id: 9,
                title: "News",
                active: false,
                url: '#'
            },
            {
                id: 10,
                title: "Shop",
                active: false,
                url: '#'
            },
        ]
        }
    }
}
</script>

<template>
<header>
    <section>
        <nav>
            <img src="/img/dc-logo.png" alt="Logo DC Comics">
        </nav>
        <nav>
            <ul>
                <li v-for="item in headerLink" :key="item.id">
                    {{item.title}}
                </li>
            </ul>
        </nav>
    </section>
</header>
</template>

<style lang="scss" scoped>
    @use '../styles/parziali/variabili'  as *;
    @use '../styles/parziali/mixins' as*;

    section{
        display: flex;
        justify-content: space-around;
        align-items: center;
        width: 100vw;
        height: 4rem;
    }

    nav img {
        width: 50px;
    }

    nav ul {
        @include my_d_flex;
    }

    nav ul li {
        text-transform: uppercase;
        margin-left: 1rem;
        font-size: .6rem;

        &:hover {
            color: $color_text;
        }
    }
</style>