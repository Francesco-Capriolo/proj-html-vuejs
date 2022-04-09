<template>
  <section class="row bg-light">
    <div class="container-fluid position-relative pb-5 mb-5">
      <h3 class="pt-5 fw-bold text-center">Popular Courses</h3>
      <p class="text-secondary text-center">
        Discover our most popular courses for self learning
      </p>
      <div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 row-cols-lg-6 g-4">
        <div
          class="col"
          v-for="(element, index) in courses"
          :key="index + 'Courses'"
          :class="index == activeElement ? 'active' : ''"
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
              class="
                border-top
                d-flex
                justify-content-between
                align-items-center
              "
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
      <div class="position-absolute bottom-0 start-50 p-2 translate-middle-x">
        <span class="p-1 bg-light border" @click="prev()"
          ><i class="fas fa-angle-left"></i
        ></span>
        <span class="p-1 bg-light border" @click="next()"
          ><i class="fas fa-angle-right"></i
        ></span>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "IndexCarousel",
  data: function () {
    return {
      activeElement: 6,
      autoPlay: null,
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
          img: require("../../img/1561458_7f3b-272x161.jpg"),
          info: "Design",
          text: "CSS - The Complete Guide 2020(incl. Flexbox,Grid & Sass)",
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
          img: require("../../img/1208228_d61c_4-272x161.jpg"),
          info: "Design",
          text: "Digitally Painting light and Color:Amateur to Master",
          vote: 4,
          discount: "$139,99",
          price: "$70",
        },
        {
          img: require("../../img/186792_41e4_4-272x161.jpg"),
          info: "Arts & Crafts",
          text: "Android Java Masterclass - Become an App Developer",
          vote: 4,
          price: "$199.99",
        },
        {
          img: require("../../img/1776542_30b1-272x161.jpg"),
          info: "Development",
          text: "Google Searching Ninja",
          vote: 4,
          discount: "$199,99",
          price: "$95",
        },
        {
          img: require("../../img/949316_2a64_11-272x161.jpg"),
          info: "Development",
          text: "the complete IOS 10 & Swift 3 Developer Course",
          vote: 4,
          discount: "$199,99",
          price: "$100",
        },
        {
          img: require("../../img/366802_6fcc-272x161.jpg"),
          info: "Development",
          text: "Web Design for beginners:Real World Coding in HTML & CSS",
          vote: 4,
          discount: "$129,99",
          price: "$65",
        },
        {
          img: require("../../img/381588_2e6d_4-272x161.jpg"),
          info: "Development",
          text: "GitHub Ultimate: MAster GIt and GitHub- Beginner Expert",
          vote: 4,
          discount: "$99,99",
          price: "$50",
        },
        {
          img: require("../../img/838056_611a_3-272x161.jpg"),
          info: "Development",
          text: "the complete IOS 10 & Swift 3 Developer Course - Build 20 Apps",
          vote: 4,
          discount: "$199,99",
          price: "$100",
        },
        {
          img: require("../../img/1414956_d944_15-272x161.jpg"),
          info: "Development",
          text: "Android Java Masterclass - Become an App Developer",
          vote: 4,
          discount: "$99,99",
          price: "$50",
        },
        {
          img: require("../../img/1109398_4c13-272x161.jpg"),
          info: "Development",
          text: "Xamarin Forms:Build Native Cross-platform Apps with C#",
          vote: 4,
          discount: "$199,99",
          price: "$95",
        },
      ],
    };
  },
  methods: {
    next() {
      if (this.activeElement === this.courses.length - 1) {
        this.activeElement = 0;
      } else {
        this.activeElement++;
      }
    },
    prev() {
      if (this.activeElement === 0) {
        this.activeElement = this.courses.length - 1;
      } else {
        this.activeElement--;
      }
    },
  },
};
</script>

<style lang="scss" scoped>
.container-fluid {
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
.position-absolute {
  cursor: pointer;
}
.active {
  display: block;
}
</style>