<template>
  <section class="row align-items-center">
    <div class="col-9 col-sm-6 col-md-5 col-lg-4 offset-md-2 p-5">
      <h3 class="fw-bolder">Investing for your Future</h3>
      <p>
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Sapiente,
        numquam saepe veniam id sit corporis temporibus facilis aspernatur quo
        neque eveniet tempore tenetur, recusandae natus ipsum provident maiores
        perspiciatis repudiandae!
      </p>
      <p class="m-0 fw-bold">Linda Green</p>
      <span>Product Manager,Apple Inc</span>
    </div>
  </section>
</template>

<script>
export default {
  name: "BannerFuture",
};
</script>

<style lang="scss" scoped>
section {
  background-image: url("../../img/testimonial-1-1917x640-1-1914x639.jpg");
  height: 500px;
  background-position: center center;
  background-repeat: no-repeat;
  background-size: cover;
  div {
    background-color: white;
    height: 70%;
  }
  span {
    font-size: 12px;
  }
}
</style>