<template>
  <div class="row top-header align-items-center justify-content-between">
    <div class="col-2 text-start">
      <span>English<i class="fas fa-angle-down"></i></span>
    </div>
    <div class="col-6 text-end">
      <div class="d-inline me-2">
        <span v-for="string in topHeader" :key="string" class="top-search"
          >{{ string }}
        </span>
      </div>
      <div class="d-inline">
        <i v-for="n in links" :key="n" :class="n"></i>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TopHeader",
  props: ["list"],
  data: function () {
    return {
      links: [
        "fab fa-facebook",
        "fab fa-twitter",
        "fab fa-instagram",
        "fab fa-linkedin",
        "fab fa-youtube",
      ],
      topHeader: ["Home", "Pages", "Course Formats", "Couses", "Demos"],
    };
  },
};
</script>

<style lang="scss" scoped>
.top-header {
  margin: 0 auto;
  width: 90%;
  font-size: 12px;
  color: grey;
  height: 4vh;
  border-bottom: 1px solid lightgray;
}
i {
  margin: 0 0.3rem;
  cursor: pointer;
}
</style>