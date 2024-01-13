<script>
import HeaderApp from './components/HeaderApp.vue';
import FooterApp from './components/FooterApp.vue';
import MainApp from './components/MainApp.vue';
export default {
  components: {
    HeaderApp,
    FooterApp,
    MainApp
  }

}
</script>
<template lang="">
  <div>
    <HeaderApp />
    <MainApp />
    <FooterApp />

  </div>
</template>

<style lang="scss">
@use './styles/partials/variables' as *;
@use './styles/generals.scss' as *;
</style>