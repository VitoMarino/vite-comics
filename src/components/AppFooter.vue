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
        <nav class="nav-prima">
            <ul>
            <li>
                <h3>
                    DC COMICS
                </h3>
            </li>
            <li v-for="item in linkDcComics" :key="item.id">
                {{ item.title }}
            </li>
            <!--SHOP-->
            <li>
                <h3>
                    SHOP
                </h3>
            </li>
            <li v-for="item in linkShop" :key="item.id">
                {{ item.title }}
            </li>
        </ul>

        <ul>
            <li>
                <h3>
                    DC
                </h3>
            </li>   
            <li v-for="item in linkSites" :key="item.id">
                {{ item.title }}
            </li>
        </ul>

        <ul>
            <li>
                <h3>
                    SITES
                </h3>
            </li>
            <li v-for="item in linkDc" :key="item.id">
                {{ item.title }}
            </li>
        </ul>

        <ul>
            <li>
                <img class="li-img" src="/img/dc-logo-bg.png" alt="Logo DC">
            </li>
        </ul>
        
    </nav>
    </section>

    <section>
        <nav class="nav-footer-social">
            <ul>
            <button>
                SIGN-UP NOW!
            </button>
        </ul>
        <ul>
            <li>
                Follow Us
            </li>
        </ul>

        <div class="div-social">
            <img src="/img/footer-facebook.png" alt="Facebook">
            <img src="/img/footer-twitter.png" alt="Twitter ma ora si chiama X">
            <img src="/img/footer-youtube.png" alt="YouTube">
            <img src="/img/footer-pinterest.png" alt="Pinterest">
            <img src="/img/footer-periscope.png" alt="Periscope">
        </div>
        </nav>
    </section>

    <section class="footer-finale">
    
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
        color:#525553;
    }

    nav ul li h3 {
        color: white;
    }

    nav.nav-prima ul li {
        margin: .5rem;
    }

    nav.nav-prima{
        display: flex;
        justify-content: center;
        padding-top: 2rem;
        font-size: .5rem;
    }

    img.li-img {
        width: 200px;
        margin-left: 10rem;
    }

    nav.nav-footer-social{
        height: 5rem;
        background-color: $bg_color_grey;
        font-size: .8rem;
        text-transform: uppercase;
        color: $color_text;
        display: flex;
        justify-content: space-around;
        align-items: center;
    }

    section.footer-finale{
        background-color: $bg_color_black;
        width: 100vw;
        height: 8rem;
    }

    button{
        @include button;
    }

    div.div-social img{
        margin-right: .8rem;

        &:hover {
            background-color: white;
            border-radius: 2rem;
            padding: .2rem;
        }
    }
</style>