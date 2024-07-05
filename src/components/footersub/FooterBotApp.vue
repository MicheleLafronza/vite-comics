<script>

    export default {
        name: "FooterBotApp",
        data() {
            return {

            }
        }
    }

</script>

<template>

    <div class="container">

        <div class="sign-up">
            <a href="">
                SIGN-UP NOW!
            </a>
        </div>

        <div class="links-container">
            <a class="link-text" href="">FOLLOW US</a>
            <a class="link-icons" href="#">
                <img src="../../assets/footer-facebook.png" alt="">
            </a>
        </div>
    </div>

</template>

<style lang="scss" scoped>
.container {
    display: flex;
    justify-content: space-between;
    position: relative;
}

.sign-up {
    padding-top: 30px;
    padding-bottom: 30px;

    a {
        padding: 8px;
        border: solid 3px rgba(8,119,222,255);
        text-decoration: none;
        color: white;
    }
}

.links-container {

    display: flex;
    gap: 10px;
    align-items: center;

    .link-text {
    color: rgba(2,130,249,255);
    text-decoration: none;
    font-size: 1.2rem;
    }
}
</style>