<template>
  <section>
    <JumboMain />
    <PopularCourses />
    <BannerLearn />
    <RecentCourses />
    <Carousel />
  </section>
</template>

<script>
import JumboMain from "./JumboMain.vue";
import PopularCourses from "./PopularCourses.vue";
import BannerLearn from "./BannerLearn.vue";
import Carousel from "./Carousel.vue";
import RecentCourses from "./RecentCourses.vue";

export default {
  name: "IndexMain",
  components: {
    JumboMain,
    PopularCourses,
    BannerLearn,
    RecentCourses,
    Carousel,
  },
};
</script>

<style lang="scss" scoped>
</style>