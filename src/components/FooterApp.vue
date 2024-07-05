<script>
import FooterTopApp from './footersub/FooterTopApp.vue';

export default {
    name: "FooterApp",
    components: {
        FooterTopApp,
    }

}

</script>

<template>
    <footer>
        
        <FooterTopApp />
        
    </footer>
</template>

<style lang="scss" scoped>
footer {
    background-color: rgba(2,130,249,255);
}
</style>