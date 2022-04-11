<template>
  <section>
    <JumboMain />
    <PopularCourses />
    <BannerLearn />
    <RecentCourses />
    <Subscribe />
    <Carousel />
    <StartDoing />
    <BannerFuture />
  </section>
</template>

<script>
import JumboMain from "./bannerComponents/JumboMain.vue";
import PopularCourses from "./sectionsMain/PopularCourses.vue";
import BannerLearn from "./bannerComponents/BannerLearn.vue";
import Carousel from "./sectionsMain/Carousel.vue";
import RecentCourses from "./sectionsMain/RecentCourses.vue";
import Subscribe from "./sectionsMain/Subscribe.vue";
import StartDoing from "./sectionsMain/StartDoing.vue";
import BannerFuture from "./bannerComponents/BannerFuture.vue";

export default {
  name: "IndexMain",
  components: {
    JumboMain,
    PopularCourses,
    BannerLearn,
    RecentCourses,
    Subscribe,
    Carousel,
    StartDoing,
    BannerFuture,
  },
};
</script>

<style lang="scss" scoped>
</style>