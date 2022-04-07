<template>
  <section class="container-fluid">
    <div class="row top-header align-items-center">
      <div class="col-2">
        <span>English<i class="fas fa-angle-down"></i></span>
      </div>
      <div class="d-flex col-10 text-end">
        <div class="col-10">
          <span v-for="string in topHeader" :key="string" class="top-search"
            >{{ string }}
          </span>
        </div>
        <div class="col-2">
          <i v-for="n in links" :key="n" :class="linkSecondaryNav.icona"></i>
          <i class="fab fa-twitter"></i>
          <i class="fab fa-instagram"></i>
          <i class="fab fa-linkedin"></i>
          <i class="fab fa-youtube"></i>
        </div>
      </div>
    </div>
    <div class="row search-header">
      <div class="col-2 d-flex align-items-center">
        <img
          class="img-fluid"
          src="../img/footer-logo2x-50x56.png"
          alt="Master Study"
        />
        <span class="text-uppercase"><b>Master</b>Study</span>
      </div>
      <div class="col-5 d-flex align-items-center">
        <label class="text-uppercase me-1" for="input">
          <i class="fas fa-bars"></i>
          category
        </label>
        <div class="input-group flex-nowrap">
          <input
            type="text"
            class="form-control"
            placeholder="Search courses"
          />
          <span class="input-group-text">
            <i class="fas fa-search"></i>
          </span>
        </div>
      </div>
      <div class="col-3 d-flex align-items-center">
        <span><i class="fas fa-bullhorn"></i>Become an Instructor</span>
        <span><i class="fas fa-briefcase"></i>For enterprise</span>
      </div>
      <div class="col-2 d-flex align-items-center">
        <span><i class="far fa-user"></i>Log in</span>
        <button class="bg-danger btn-lg rounded-pill">Sign Up</button>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "IndexHeader",
  data: function () {
    return {
      links: ["fab fa-facebook"],
      topHeader: ["Home", "Pages", "Course Formats", "Couses", "Demos"],
    };
  },
};
</script>

<style lang="scss" scoped>
.row {
  padding: auto 0;
}
.top-header {
  font-size: 12px;
  color: grey;
  height: 4vh;
  border-bottom: 1px solid lightgray;
}
.top-search {
  margin: 0 0.3rem;
}
i {
  margin: 0 0.3rem;
}
img {
  filter: url("#red-sunset-with-purple");
}
label {
  font-size: 12px;
}
.input-group {
  width: 80%;
  input {
    background-color: #f0f2f5;
  }
}
.input-group-text {
  background-color: #457992;
  i {
    color: white;
  }
}
.search-header {
  height: 8vh;
}
</style>