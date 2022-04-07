<template>
  <section class="row search-header">
    <div class="col-2 d-flex align-items-center">
      <img
        class="img-fluid"
        src="../img/footer-logo2x-50x56.png"
        alt="Master Study"
      />
      <p class="text-uppercase text-black mb-0"><b>Master</b>Study</p>
    </div>
    <div class="col-5 d-flex align-items-center">
      <span class="text-uppercase me-2" for="input">
        <i class="fas fa-bars"></i>
        category
      </span>
      <div class="input-group flex-nowrap">
        <input type="text" class="form-control" placeholder="Search courses" />
        <span class="input-group-text">
          <i class="fas fa-search"></i>
        </span>
      </div>
    </div>
    <div class="col-3 d-flex align-items-center">
      <span><i class="fas fa-bullhorn"></i>Become an Instructor</span>
      <span><i class="fas fa-briefcase"></i>For enterprise</span>
    </div>
    <div class="col-2 d-flex align-items-center justify-content-end">
      <span class="me-2"><i class="far fa-user"></i>Log in</span>
      <button class="btn btn-danger rounded-pill">Sign Up</button>
      <i class="far fa-bookmark ms-2"></i>
    </div>
  </section>
</template>

<script>
export default {
  name: "SearchHeader",
};
</script>

<style lang="scss" scoped>
.row {
  padding: auto 0;
}
.search-header {
  height: 8vh;
  span {
    font-size: 12px;
    color: gray;
  }
  i {
    margin: 0 0.5rem;
    color: gray;
  }
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
img {
  filter: url("#red-sunset-with-purple");
}
</style>