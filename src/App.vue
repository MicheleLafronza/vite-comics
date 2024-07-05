<script>
import HeaderApp from './components/HeaderApp.vue';
import ContentApp from './components/ContentApp.vue';
export default {
  components: {
    HeaderApp,
    ContentApp,
  }
}
</script>

<template>
  <HeaderApp />

  <ContentApp />
  
</template>

<style lang="scss">
@use './style/general.scss' as *;
</style>
