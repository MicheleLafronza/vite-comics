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
                    <a href="#"><span>{{ link.text }}</span></a>
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
    gap: 20px;

    li {
        cursor: pointer;
        position: relative;

        a {
            height: 123px;
            display: flex;
            align-items: center;
            text-decoration: none;
            color: black;
            
            
            &:hover {
                color: rgba(2,130,249,255);
                border-bottom: 3px solid rgba(2,130,249,255);
            }

        }
    }
}
</style>