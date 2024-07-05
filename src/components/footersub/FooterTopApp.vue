<script>

export default {
    name: "FooterTopApp",
    data() {
        return {
            links: [
                {
                    text: "DIGITAL COMICS",
                    image: "/src/assets/buy-comics-digital-comics.png"
                },
                {
                    text: "DC MERCHANDISE",
                    image: "/src/assets/buy-comics-merchandise.png"
                },
                {
                    text: "SUBSCRIPTION",
                    image: "/src/assets/buy-comics-subscriptions.png"
                },
                {
                    text: "COMIC SHOP LOCATOR",
                    image: "/src/assets/buy-comics-shop-locator.png"
                },
                {
                    text: "DC POWER VISA",
                    image: "/src/assets/buy-dc-power-visa.svg"
                }
            ]
        }
    }
}

</script>

<template>

    <div class="container">
        <ul>
            <li v-for="(link, index) in links" :key="index">
                <img class="link-img" :src="link.image" alt="">
                <a href="">
                    {{ link.text }}
                </a>
            </li>    
        </ul>

    </div>
        

</template>

<style lang="scss" scoped>

.container {
    padding: 50px;
}
ul {
    list-style-type: none;
    display: flex;
    justify-content: space-around;
    gap: 10px;
}

img {
    display: block;
}

a {
    color: white;
    text-decoration: none;
}

.link-img {
    float: left;
    width: 50px;
    
}

li {
    display: flex;
    align-items: center;
    gap: 10px;
    cursor: pointer;
}
</style>