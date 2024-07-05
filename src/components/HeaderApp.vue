<script>

    export default {
        name: "HeaderApp",
        data() {
        return {
            links: [
            {
                text: "CHARACTERS"
            },
            {
                text: "COMICS"
            },
            {
                text: "MOVIES"
            },
            {
                text: "TV"
            },
            {
                text: "GAMES"
            },
            {
                text: "COLLECTIBLES"
            },
            {
                text: "VIDEOS"
            },
            {
                text: "FANS"
            },
            {
                text: "NEWS"
            },
            {
                text: "SHOP"
            },
            ]
        }
    }
    };

    

</script>

<template>

<header>

    <div class="container">
        <div class="logo">
            <img src="../assets/dc-logo.png" alt="logo header">
        </div>
        
        <div class="menu">
            <ul>
                <li v-for="(link, index) in links" :key="index">
                    {{ link.text }}
                </li>
            </ul>
        </div>
    </div>

</header>

</template>

<style lang="scss" scoped>
@use '/src/style/partials/variables' as *;


header {
    background-color: $white;
}

.container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    padding: 20px;

    img {
        width: 80px;
    }
}

ul {
    list-style-type: none;
    display: flex;
    justify-content: space-between;
    gap: 10px;

    li {
        cursor: pointer;
    }
}
</style>