<script>
export default {
  data() {
    return {
      products: [
        {
          url: "#",
          img: "buy-comics-digital-comics.png",
          text: "DIGITAL COMICS",
        },
        {
          url: "#",
          img: "buy-comics-merchandise.png",
          text: "DC MERCHANDISE",
        },
        {
          url: "#",
          img: "buy-comics-subscriptions.png",
          text: "SUBSCRIPTION",
        },
        {
          url: "#",
          img: "buy-comics-shop-locator.png",
          text: "COMIC SHOP LOCATOR",
        },
        {
          url: "#",
          img: "buy-dc-power-visa.svg",
          text: "DC POWER VISA",
        },
      ],
    };
  },
};
</script>

<template>
  <aside>
    <div class="container">
      <section v-for="product in products" :key="product.text">
        <img :src="'src/assets/img/' + product.img" alt="" />

        <p>{{ product.text }}</p>
      </section>
    </div>
  </aside>
</template>

<style lang="scss" scoped>
@use "../assets/scss/partials/mixins.scss" as *;

aside {
  height: 7rem;
  color: white;
  line-height: 7rem;
  background-color: #0082f9;
  display: flex;
  font-size: 0.8rem;
  font-weight: 600;
  div {
    display: flex;
    justify-content: space-evenly;
  }
  section {
    @include my-flex-center(both);
    display: flex;
    img {
      height: 2.5rem;
      margin-right: 1rem;
    }
  }
  section:last-child {
    img {
      height: 1.8rem;
    }
  }
}
</style>
