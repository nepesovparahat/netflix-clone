<template>
  <div class="home">
    <Hero :params="paramsUrl[2]" />
    <div class="home__swiper">
      <MovieSwiper
        :params="params"
        v-for="params in paramsUrl"
        :key="params.id"
      />
    </div>
  </div>
</template>

<script>
import MovieSwiper from "@/components/swiper/MovieSwiper.vue";
import Hero from "@/components/hero/Hero.vue";
export default {
  name: "Home",
  components: {
    MovieSwiper,
    Hero,
  },
  setup() {
    let paramsUrl = [
      { title: "Romance", genres: 10749 },
      { title: "Thriller", genres: 53 },
      { title: "Horror", genres: 27 },
      { title: "Top Rated", genres: 35 },
    ];
    return { paramsUrl };
  },
};
</script>

<style lang="scss"></style>
