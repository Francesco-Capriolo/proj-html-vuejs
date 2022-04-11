<template>
  <section class="row">
    <div
      class="
        col-12 col-md-8
        offset-md-2
        d-flex
        flex-wrap
        text-white
        align-items-center
        justify-content-center
      "
    >
      <div class="col-12 col-md-6 col-lg-3 p-2 my-height">
        <h4 class="text-uppercase">About</h4>
        <p>
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. Reiciendis
          ex laboriosam non itaque, libero dolorum quaerat obcaecati iusto
          perspiciatis sit neque sequi voluptates magnam est iure quia minus
          ipsa voluptate!
        </p>
      </div>
      <div class="col-12 col-md-6 col-lg-3 p-2 my-height">
        <h4 class="text-uppercase">Contact</h4>
        <p>Usa, California 20, First Avenue,California</p>
        <p class="m-0">Tel.:+1 212 435 666 22</p>
        <p>Fax:+1 212 334 56 46</p>
        <span class="text-secondary">Info@masterstudy.com</span>
      </div>
      <div class="col-12 col-md-6 col-lg-3 p-2 my-height">
        <h4 class="text-uppercase">Social network</h4>
        <i class="fab fa-facebook my-circle m-2"></i>
        <i class="fab fa-instagram my-circle m-2"></i>
        <i class="fab fa-linkedin my-circle m-2"></i>
        <i class="fab fa-pinterest my-circle m-2"></i>
        <i class="fab fa-twitter my-circle m-2"></i>
        <i class="far fa-volleyball-ball my-circle m-2"></i>
        <i class="fab fa-google-plus my-circle m-2"></i>
        <i class="fab fa-skype my-circle m-2"></i>
      </div>
      <div class="col-12 col-md-6 col-lg-3 p-2">
        <img
          class="img-fluid"
          src="../img/Top-udemy-courses-90-percent-off.jpg"
          alt=""
        />
      </div>
    </div>
    <div class="row border-top">
      <div class="col-6 text-white px-5 py-3">
        <img src="../img/footer-logo2x-50x56.png" alt="" />
        <span class="ms-3"
          >Copyright 2020.
          <span class="text-decoration-underline">MasterStudy</span> theme by
          <span class="text-decoration-underline">StylemixThemes</span></span
        >
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "IndexFooter",
};
</script>

<style lang="scss" scoped>
section {
  background-color: #273044;
  padding: 2rem 0 1rem;
  .my-height {
    min-height: 230px;
  }
  .my-circle {
    border-radius: 50%;
    padding: 0.8rem 0.8rem;
  }
  .fa-facebook {
    background-color: darkblue;
  }
  .fa-instagram {
    background-color: magenta;
  }
  .fa-linkedin {
    background-color: rgb(3, 53, 218);
  }
  .fa-pinterest {
    background-color: red;
  }
  .fa-twitter {
    background-color: rgb(0, 162, 255);
  }
  .fa-google-plus {
    background-color: orange;
  }
  .fa-skype {
    background-color: aqua;
  }
  div.border-top {
    height: 50px;
    margin: 0 auto;
    img {
      height: 30px;
      width: 30px;
    }
  }
}
</style>