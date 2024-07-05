<script>
import HeaderApp from './components/HeaderApp.vue';
import ContentApp from './components/ContentApp.vue';
import FooterApp from './components/FooterApp.vue';
export default {
  components: {
    HeaderApp,
    ContentApp,
    FooterApp,
  }
}
</script>

<template>
  <HeaderApp />

  <ContentApp />

  <FooterApp />
</template>

<style lang="scss">
@use './style/general.scss' as *;
</style>
