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
import JumboMain from "./bannerComponents/JumboMain.vue";
import PopularCourses from "./sectionsMain/PopularCourses.vue";
import BannerLearn from "./bannerComponents/BannerLearn.vue";
import Carousel from "./sectionsMain/Carousel.vue";
import RecentCourses from "./sectionsMain/RecentCourses.vue";

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