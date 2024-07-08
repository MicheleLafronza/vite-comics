<script>
    export default {
        name: "FooterMidApp",
        data() {
            return {
                comicsLinks: [
                    {
                        text: "Characters"
                    },
                    {
                        text: "Comics"
                    },
                    {
                        text: "Movies"
                    },
                    {
                        text: "TV"
                    },
                    {
                        text: "Games"
                    },
                    {
                        text: "Videos"
                    },
                    {
                        text: "News"
                    },

                ],

                shopLinks: [
                    {
                        text: "Shop DC"
                    },
                    {
                        text: "Shop DC Collectibles"
                    }
                ],

                DCLinks: [
                    {
                        text: "Term of use"
                    },
                    {
                        text: "Privacy Policy"
                    },
                    {
                        text: "Ad Choiches"
                    },
                    {
                        text: "Advertising"
                    },
                    {
                        text: "Jobs"
                    },
                    {
                        text: "Subrscriptions"
                    },
                    {
                        text: "Talent Workshops"
                    },
                    {
                        text: "CPSC Certificates"
                    },
                    {
                        text: "Ratings"
                    },
                    {
                        text: "Shop Help"
                    },
                    {
                        text: "Contact Us"
                    }
                ],

                siteLinks: [
                    {
                        text: "DC"
                    },
                    {
                        text: "MAD Magazine"
                    },
                    {
                        text: "DC Kids"
                    },
                    {
                        text: "DC Universe"
                    },
                    {
                        text: "DC PowerVisa"
                    }
                ]
            }
        }
    }

</script>

<template>
    <div class="container">

        <div class="links">

            <div class="links-sections">
                <span class="list-title">
                    DC COMICS
                </span>
                <ul>
                    <li v-for="(link, index) in comicsLinks" :key="index">
                    {{ link.text }}
                    </li>
                </ul>
            </div>

            <div class="links-sections">
                <span class="list-title">
                    SHOP
                </span>
                <ul>
                    <li v-for="(link, index) in shopLinks" :key="index">
                    {{ link.text }}
                    </li>
                </ul>
            </div>

            <div class="links-sections">
                <span class="list-title">
                    DC
                </span>
                <ul>
                    <li v-for="(link, index) in DCLinks" :key="index">
                    {{ link.text }}
                    </li>
                </ul>
            </div>
            
            <div class="links-sections">
                <span class="list-title">
                    SITES
                </span>
                <ul>
                    <li v-for="(link, index) in siteLinks" :key="index">
                    {{ link.text }}
                    </li>
                </ul>
            </div>
        </div>

        <div class="bg-logo">
            <img src="../../assets/dc-logo-bg.png" alt="">
        </div>

    </div>    
</template>

<style lang="scss" scoped>

.container {
    display: flex;
    justify-content: space-between;

}

.links {
    flex-basis: 35%;
    padding-top: 20px;
    padding-left: 20px;
    color: white;
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    height: 400px;
}

.list-title {
    font-size: 1.5rem;
    margin-top: 10px;
    margin-bottom: 10px;
    display: inline-block;
}

ul {
    list-style-type: none;
}

li {
    padding: 5px;
    color: grey;
    cursor: pointer;
}

.bg-logo {
    flex-basis: 40%;
    position: relative;
    z-index: 0;
}

img {
    height: 115%;
    position: absolute;
    top: -25px;
    bottom: -25px;
    z-index: 0;
    max-width: 100%;
}

</style>