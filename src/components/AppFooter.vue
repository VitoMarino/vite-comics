<script>
export default{
    data() {
        return {
            linkDcComics : [
            {
                id: 1,
                title: "Characters",
                active: false,
            },
            {
                id: 2,
                title: "Comics",
                active: false,
            },
            {
                id: 3,
                title: "Movies",
                active: false,
            },
            {
                id: 4,
                title: "TV",
                active: false,
            },
            {
                id: 5,
                title: "Games",
                active: false,
            },
            {
                id: 6,
                title: "Videos",
                active: false,
            },
            {
                id: 7,
                title: "News",
                active: false,
            },
        ],

        linkShop: [
            {
                id: 24,
                title: "Shop DC",
                active: false,
            },
            {
                id: 25,
                title: "Shop DC Collectibles",
                active: false,
            },    
        ],

        linkDc : [
                {
                id: 8,
                title: "Terms of Use",
                active: false,
            },
            {
                id: 9,
                title: "Privacy policy (New)",
                active: false,
            },
            {
                id: 10,
                title: "Ad Choices",
                active: false,
            },
            {
                id: 11,
                title: "Advertising",
                active: false,
            },
            {
                id: 12,
                title: "Jobs",
                active: false,
            },
            {
                id: 13,
                title: "Subscriptions",
                active: false,
            },
            {
                id: 14,
                title: "Talent Workshops",
                active: false,
            },
            {
                id: 15,
                title: "CPSC Cerificates",
                active: false,
            },
            {
                id: 16,
                title: "Ratings",
                active: false,
            },
            {
                id: 17,
                title: "Shop Help",
                active: false,
            },
            {
                id: 18,
                title: "Contact Us",
                active: false,
            },
        ],

        linkSites : [
            {
                id: 19,
                title: "DC",
                active: false,
            },
            {
                id: 20,
                title: "MAD magazine",
                active: false,
            },
            {
                id: 21,
                title: "DC Kids",
                active: false,
            },
            {
                id: 22,
                title: "DC Universe",
                active: false,
            },
            {
                id: 23,
                title: "DC Power Visa",
                active: false,
            },
        ],
        }    
    }
}
</script>

<template>
<footer>
    <section class="primo-Footer">
        <nav>
            <ul class="primo-ul">
            <li>
                <h3>
                    DC COMICS
                </h3>
            </li>
            <li v-for="item in linkDcComics" :key="item.id">
                {{ item.title }}
            </li>
        </ul>

        <ul class="secondo-ul">
            <li>
                <h3>
                    SHOP
                </h3>
            </li>
            <li v-for="item in linkShop" :key="item.id">
                {{ item.title }}
            </li>
        </ul>

        <ul class="terzo-ul">
            <li>
                <h3>
                    DC
                </h3>
            </li>   
            <li v-for="item in linkSites" :key="item.id">
                {{ item.title }}
            </li>
        </ul>

        <ul class="quarto-ul">
            <li>
                <h3>
                    SITES
                </h3>
            </li>
            <li v-for="item in linkDc" :key="item.id">
                {{ item.title }}
            </li>
        </ul>
        </nav>
        
    </section>

    <section class="Subscribe">
        <ul>
            <button>
                SIGN-UP NOW!
            </button>
        </ul>
        <ul>

        </ul>
    </section>

    <section>

    </section>
</footer>
</template>

<style lang="scss" scoped>
    @use '../styles/parziali/variabili'  as *;
    @use '../styles/parziali/mixins' as*;

    section.primo-Footer {
        background-image: url(/img/footer-bg.jpg);
        background-repeat: no-repeat;
        height: 16.5rem;
        color: white;
    }

    nav{
        display: flex;
    }



</style>