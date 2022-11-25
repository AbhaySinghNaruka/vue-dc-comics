<template>
  <div>
    <footer>
      <div class="footer-container">
        <div class="links">
          <div class="footer-links"></div>
          <div class="footer-logo">
            <img class="logo-tilted" src="@/assets/img/dc-logo-bg.png" alt="">
          </div>
        </div>
      </div>
    </footer>
    <div class="black"></div>
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
      width: 30%;
      background-color: cadetblue;
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
  height: 115px;
}

</style>
