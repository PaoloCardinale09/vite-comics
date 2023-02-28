<script>
import AppHeader from "./components/AppHeader.vue";
import AppFooter from "./components/AppFooter.vue";
import AppMain from "./components/AppMain.vue";
import AppAside from "./components/AppAside.vue";
import AppJumbotron from "./components/AppJumbotron.vue";
export default {
  data() {
    return {};
  },

  components: { AppHeader, AppFooter, AppMain, AppAside, AppJumbotron },
};
</script>

<template>
  <AppHeader />
  <AppJumbotron />
  <AppMain />
  <AppAside />
  <AppFooter />
</template>

<style lang="scss">
@use "./assets/scss/general.scss";
</style>
