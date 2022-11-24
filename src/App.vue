<template>
  <div>
    <HeaderPage />
    <FooterPage />
  </div>
</template>

<script>
import HeaderPage from '@/components/HeaderPage.vue';
import FooterPage from '@/components/FooterPage.vue';

export default {
  components: {
    HeaderPage,
    FooterPage,
  },
};
</script>

<style lang="scss">
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Montserrat', sans-serif;
  }

</style>
