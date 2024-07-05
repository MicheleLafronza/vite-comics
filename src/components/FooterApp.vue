<script>
import FooterMidApp from './footersub/FooterMidApp.vue';
import FooterTopApp from './footersub/FooterTopApp.vue';

export default {
    name: "FooterApp",
    components: {
        FooterTopApp,
        FooterMidApp,
    }

}

</script>

<template>

    <div class="footer-top">
        <FooterTopApp />
    </div>

    <div class="footer-mid">
        <FooterMidApp />
    </div>

    <div class="footer-bottom">

    </div>
        
</template>

<style lang="scss" scoped>
.footer-top {
    background-color: rgba(2,130,249,255);
}

.footer-mid {
    background: url(../assets/footer-bg.jpg);
}

.footer-bottom {
    background-color: rgba(48,48,48,255);
}
</style>