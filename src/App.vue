<script>
import AppHeader from "./components/AppHeader.vue";
import AppFooter from "./components/AppFooter.vue";
import AppMain from "./components/AppMain.vue";
export default {
  data() {
    return {
      title: "Hello world!!",
    };
  },

  components: { AppHeader, AppFooter, AppMain },
};
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppFooter />
</template>

<style scoped></style>
