<template>
  <div class="card">
    <div class="contents">
      <img
        :src="movie.thumb"
        :alt="movie.titolo"
      >
      <h2>{{ movie.titolo }}</h2>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CardMovie',
  props: {
    movie: Object,
  },
};
</script>

<style lang="scss" scoped>
  .card {
    text-align: center;
    padding: .1rem;
    .contents {
      background-color: white;
      padding: 1em;
      height: 100%;
      img {
        max-width: 90%;
      }
      h2 {
        font-size: 1.2rem;
      }
    }
  }
</style>
