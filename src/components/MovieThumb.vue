<template>
  <div>
    <router-link :to="`/movie/${movie.imdbID}`" class="q-pa-md">
        <div class="movie">
          <q-img
            :src="movie.Poster"
            :ratio="0.69"
            spinner-color="primary"
            spinner-size="82px"
          />
          <div class="title q-mt-md">{{ movie.Title }}</div>
        </div>
    </router-link>
  </div>
</template>

<script>
export default {
  props: {
    movie: Object,
  },
};
</script>

<style lang="scss" scoped>
.movie {
  padding: 20px;
}
a {
  text-align: center;
  color: white;
  text-decoration: none;
}

</style>