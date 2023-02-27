<script>
import AppHeader from "./components/AppHeader.vue";
import AppFooter from "./components/AppFooter.vue";
import AppMain from "./components/AppMain.vue";
import AppAside from "./components/AppAside.vue";
export default {
  data() {
    return {
      title: "Hello world!!",
    };
  },

  components: { AppHeader, AppFooter, AppMain, AppAside },
};
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppAside />
  <AppFooter />
</template>

<style lang="scss">
@use "./assets/scss/general.scss";
</style>
