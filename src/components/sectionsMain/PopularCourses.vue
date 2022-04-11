<template>
  <section class="container-fluid mb-5">
    <p class="pt-5 fw-bold">Popular Development Courses</p>
    <div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 row-cols-lg-6 g-4">
      <div
        class="col"
        v-for="(element, index) in courses"
        :key="index + 'popular'"
      >
        <div class="card">
          <img :src="element.img" class="card-img-top" alt="element.text" />
          <div class="card-body">
            <h5 class="card-title">
              {{ element.info }}<i class="fas fa-angle-right"></i>
            </h5>
            <p class="card-text">
              {{ element.text }}
            </p>
          </div>
          <div
            class="border-top d-flex justify-content-between align-items-center"
          >
            <div>
              <span v-for="n in element.vote" :key="n">
                <i class="fas fa-star"></i>
              </span>
            </div>
            <div>
              <span
                class="
                  discount
                  text-decoration-line-through text-secondary
                  d-block
                "
                >{{ element.discount }}</span
              >
              <span>{{ element.price }}</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "PopularCouses",
  data: function () {
    return {
      courses: [
        {
          img: require("../../img/895786_7b4b_2-272x161.jpg"),
          info: "Development",
          text: "the complete IOS 10 & Swift 3 Developer Course",
          vote: 4,
          discount: "$199,99",
          price: "$100",
        },
        {
          img: require("../../img/246154_d8b0_3-272x161.jpg"),
          info: "Development",
          text: "Web Design for beginners:Real World Coding in HTML & CSS",
          vote: 4,
          discount: "$129,99",
          price: "$65",
        },
        {
          img: require("../../img/752950_b773-272x161.jpg"),
          info: "Development",
          text: "GitHub Ultimate: MAster GIt and GitHub- Beginner Expert",
          vote: 4,
          discount: "$99,99",
          price: "$50",
        },
        {
          img: require("../../img/1253188_58f7_2-272x161.jpg"),
          info: "Development",
          text: "the complete IOS 10 & Swift 3 Developer Course - Build 20 Apps",
          vote: 4,
          discount: "$199,99",
          price: "$100",
        },
        {
          img: require("../../img/919872_ed54_6-272x161.jpg"),
          info: "Development",
          text: "Android Java Masterclass - Become an App Developer",
          vote: 4,
          discount: "$99,99",
          price: "$50",
        },
        {
          img: require("../../img/951684_9c1a_2-272x161.jpg"),
          info: "Development",
          text: "Xamarin Forms:Build Native Cross-platform Apps with C#",
          vote: 4,
          discount: "$199,99",
          price: "$95",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
section {
  margin: 0 auto;
  width: 90%;
  .card {
    padding: 0;
    cursor: pointer;
  }
  .fw-bold {
    padding: 0;
  }
  .card-title {
    font-size: 10px;
    color: lightgray;
  }
  .card-text {
    font-size: 12px;
  }
  .fa-star {
    font-size: 10px;
    color: gold;
  }
  .discount {
    font-size: 10px;
  }
  .border-top {
    padding: 0.5rem;
  }
}
</style>