<template>
  <div>
    <footer>
      <div class="footer-container">
        <div class="links">
          <div class="footer-links">
            <ul>
              <li class="link-title">DC COMICS</li>
              <li>Characters</li>
              <li>Comics</li>
              <li>Movies</li>
              <li>TV</li>
              <li>Games</li>
              <li>Video</li>
              <li>News</li>
              <li class="link-title">SHOP</li>
              <li>Shop DC</li>
              <li>Shop DC Collectibles</li>
            </ul>
            <ul>
              <li class="link-title">DC</li>
              <li>Terms Of Use</li>
              <li>Privacy policy (New)</li>
              <li>Ad Choices</li>
              <li>Advertising</li>
              <li>Jobs</li>
              <li>Subscriptions</li>
              <li>Talent Workshops</li>
              <li>CPSC Certificates</li>
              <li>Ratings</li>
              <li>Shop Help</li>
              <li>Contact Us</li>
            </ul>

            <ul>
              <li class="link-title">SITES</li>
              <li>DC</li>
              <li>MAD Magazine</li>
              <li>DC Kids</li>
              <li>DC Universe</li>
              <li>DC Power Visa</li>
            </ul>
          </div>
          <div class="footer-logo">
            <img class="logo-tilted" src="@/assets/img/dc-logo-bg.png" alt="">
          </div>
        </div>
      </div>
    </footer>
    <div class="black">
      <div class="bottom-footer-container">
        <button>SIGN-UP NOW!</button>
        <div class="right-footer">
          <ul>
            <li class="follow">FOLLOW US</li>
            <li><img src="@/assets/img/footer-facebook.png" alt=""></li>
            <li><img src="@/assets/img/footer-twitter.png" alt=""></li>
            <li><img src="@/assets/img/footer-youtube.png" alt=""></li>
            <li><img src="@/assets/img/footer-pinterest.png" alt=""></li>
            <li><img src="@/assets/img/footer-periscope.png" alt=""></li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {

};
</script>

<style lang="scss">
footer {
  height: 400px;
  background-image: url('@/assets/img/footer-bg.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  overflow: hidden;

  .footer-container {
    width: 1300px;
    margin: 0 auto;
    height: 400px;
  }

  .links {
    display: flex;
    justify-content: space-between;
    height: 100%;

    .footer-links {
      width: 50%;

      display: flex;

      .link-title {
        font-weight: bolder;
        font-size: 20px;
        color: white;
        margin-bottom: 30px;
        margin-top: 20px;
      }

      ul {
        width: 33%;
      }

      li {
        margin-bottom: 5px;
        font-size: 15px;
        color: lightgray;
      }
    }

    .footer-logo {
      width: 40%;

      position: relative;

      .logo-tilted {
        position: absolute;
        top: -80px;
      }
    }
  }
  .social-media {
    background-color: red;
    height: 25%;
  }
}

.black {
  background-color: black;
  height: 90px;

  .bottom-footer-container {
    width: 1300px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 100%;

    ul {
      color: white;
      display: flex;

      .right-footer li {
        line-height: 90px;
        height: 100%;
      }
    }
  }
}

</style>
