<script>
export default {
  props: {
    img: String,
    title: String,
  },
};
</script>
<template>
  <div class="card">
    <img :src="img" alt="img" />
    <div class="title">
      <h2>{{ title }}</h2>
    </div>
  </div>
</template>
<style lang="scss" scoped>
.container {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}
.card {
  width: calc(100% / 6);
  height: 12rem;
  padding: 1rem;
  color: white;
  margin-top: 4rem;
  margin-bottom: 1rem;
  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: top;
  }
  h2 {
    font-size: 1rem;
    margin-top: 0.5rem;
    margin-bottom: 2rem;
  }
}
</style>
