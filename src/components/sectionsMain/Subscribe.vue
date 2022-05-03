<template>
  <section
    class="row bg-danger justify-content-center align-items-center text-white"
  >
    <div class="col-12 col-md-8 d-flex flex-wrap">
      <div class="col-12 col-md-7 me-1">
        <h3>Subscribe our newsletter</h3>
        <p>
          there are many variations of passages of Lorem Ipsum avaible, but the
          majority have suffered alteration in some form, by injected humour,or
          randomised words
        </p>
      </div>
      <div
        class="
          col-12 col-md-4
          d-flex
          flex-column
          justify-content-center
          align-items-start
        "
      >
        <p class="text-uppercase">your e-mail address</p>
        <div class="input-group flex-nowrap">
          <input
            type="text"
            class="form-control"
            placeholder="enter your email"
          />
          <span class="input-group-text text-uppercase text-white">
            subscribe
          </span>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "IndexSubscribe",
};
</script>

<style lang="scss" scoped>
section {
  height: 160px;
}
p.text-uppercase {
  font-size: 12px;
  margin: 0;
}
.input-group {
  width: 75%;
  input {
    background-color: #f0f2f5;
    min-width: 120px;
  }
}
.input-group-text {
  background-color: #457992;
  cursor: pointer;
}
</style>