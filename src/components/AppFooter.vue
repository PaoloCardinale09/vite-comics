<script>
export default {
  data() {
    return {
      title: "Footer",
    };
  },
};
</script>

<template>
  <footer>
    <div class="footer--top">
      <div id="wrap" class="container">
        <div>
          <div>
            <h4>DC COMICS</h4>
            <span>Characters</span>
            <span>Comics</span>
            <span>Movies</span>
            <span>Tv</span>
            <span>Games</span>
            <span>Videos</span>
            <span>News</span>
          </div>
          <div>
            <h4>SHOP</h4>
            <span>Shop DC</span>
            <span>Shop DC Collectibles</span>
          </div>
        </div>
        <div>
          <div>
            <h4>DC</h4>
            <span>Terms Of Use</span>
            <span>Privacy policy (New)</span>
            <span>Ad Choices</span>
            <span>Advertising</span>
            <span>Jobs</span>
            <span>Subscriptions</span>
            <span>Talent Workshops</span>
            <span>CPSC Certificates</span>
            <span>Ratings</span>
            <span>Shop Help</span>
            <span>Contact US</span>
          </div>
        </div>
        <div>
          <h4>SITES</h4>
          <span>DC</span>
          <span>MAD Magazine</span>
          <span>DC Kids</span>
          <span>DC Universe</span>
          <span>Power Visa</span>
        </div>
      </div>
    </div>
    <div class="footer--bottom">
      <div class="container">
        <div class="footer--bottom-left">
          <p>SIGN-UP NOW!</p>
        </div>
        <div class="footer--bottom-right">
          <p>FOLLOW US</p>
          <img src="../assets/img/footer-facebook.png" alt="" />
          <img src="../assets/img/footer-twitter.png" alt="" />
          <img src="../assets/img/footer-youtube.png" alt="" />
          <img src="../assets/img/footer-pinterest.png" alt="" />
          <img src="../assets/img/footer-periscope.png" alt="" />
        </div>
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
@use "../assets/scss/partials/mixins.scss" as *;
.footer--top {
  height: 18rem;
  background-image: url(../assets/img/dc-logo-bg.png),
    url(../assets/img/footer-bg.jpg);
  background-repeat: no-repeat, no-repeat;
  background-size: 26rem, cover;
  background-position: 56rem -4rem, 0 0;
}
#wrap {
  display: flex;
  div {
    display: flex;
    flex-direction: column;
    margin-right: 1rem;
  }
  h4 {
    font-size: 1rem;
    color: white;
    margin: 1.5rem 1rem 0.6rem 0;
  }
  span {
    font-size: 0.6rem;
    color: #868482;
  }
}
.footer--bottom {
  height: 6rem;
  background-color: #303030;
  display: flex;
  div {
    display: flex;
    justify-content: space-between;
  }
}

.footer--bottom-left {
  @include my-flex-center(vertical);
  p {
    color: white;
    border: 2px solid #0082f6;
    font-size: 0.8rem;
    font-weight: 600;
    align-self: center;
    padding: 0.5rem;
  }
}

.footer--bottom-right {
  align-items: center;
  p {
    color: #0082f6;
    font-size: 0.8rem;
    font-weight: 600;
  }
  img {
    height: 1.5rem;
    margin-left: 1rem;
  }
}
</style>
