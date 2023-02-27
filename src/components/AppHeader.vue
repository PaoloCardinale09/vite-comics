<script>
export default {
  data() {
    return {
      title: "Header",
    };
  },
};
</script>

<template>
  <header class="container">
    <img src="../assets/img/dc-logo.png" alt="" />
    <ul>
      <li><a href="#"></a>CHARACTERS</li>
      <li><a href="#"></a>COMICS</li>
      <li><a href="#"></a>MOVIE</li>
      <li><a href="#"></a>TV</li>
    </ul>
  </header>
</template>

<style lang="scss" scoped>
@use "../assets/scss/partials/mixins.scss" as *;

header {
  height: 6rem;
  @include my-flex-center(vertical);
  justify-content: space-between;
  font-weight: 600;
  color: #514c50;
  font-size: 0.8rem;

  img {
    height: 4rem;
  }
  ul {
    display: flex;
    gap: 1rem;
  }
}
</style>
