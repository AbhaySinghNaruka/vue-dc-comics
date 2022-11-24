/* eslint-disable */
<template>
  <footer>
    <div class="footer-container">
      <div class="footer-links"></div>
      <div class="footer-logo"></div>
    </div>
    <div class="social-media">

    </div>
  </footer>
</template>

<script>
export default {

};
</script>

<style lang="scss">
footer {
  height: 500px;
  background-image: url('@/assets/img/footer-bg.jpg');

  .links {
    display: flex;
    justify-content: space-between;
    height: 75%;
    background-color: red;

    .footer-links {
      width: 30%;
      background-color: cadetblue;
    }

    .footer-logo {
      width: 30%;
      background-color: aqua;
    }
  }
}

</style>
