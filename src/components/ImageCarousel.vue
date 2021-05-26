<template>
  <div class="imgcarousel">
    <div class="top-slider">
      <VueSlickCarousel
        @beforeChange="hideMagnifier"
        ref="c1"
        :asNavFor="c2"
        :focusOnSelect="true"
        :speed="800"
      >
        <div class="block" v-for="(image, index) in images" :key="index">
          <img
            v-if="showMagnifier"
            @click="openFullscreen"
            class="magnifier"
            src="../assets/magnifier.svg"
            alt=""
          />
          <img class="image" :src="require(`../assets/${image}`)" alt="" />
        </div>
        <template #prevArrow="arrowOption">
          <div class="prev-arrow-imgcarousel">
            {{ arrowOption.currentSlide }}/{{ arrowOption.slideCount }}
          </div>
        </template>
        <template #nextArrow="arrowOption">
          <div class="next-arrow-imgcarousel">
            {{ arrowOption.currentSlide }}/{{ arrowOption.slideCount }}
          </div>
        </template>
      </VueSlickCarousel>
    </div>
    <div class="bottom-slider">
      <VueSlickCarousel
        :slidesToShow="numberOfSlides"
        ref="c2"
        :asNavFor="c1"
        :focusOnSelect="true"
        :arrows="false"
        :speed="800"
      >
        <div v-for="(image, index) in images" :key="index">
          <img :src="require(`../assets/${image}`)" alt="" />
        </div>
      </VueSlickCarousel>
    </div>
    <div class="fullscreen-image">
      <img class="new-image" alt="" />
      <span @click="closeFullscreen" class="close">&times;</span>
    </div>
  </div>
</template>

<script>
import VueSlickCarousel from "vue-slick-carousel";

export default {
  name: "ImageCarousel",
  data: () => ({
    numberOfSlides: 7,
    showMagnifier: true,
    images: [
      "img1.jpg",
      "img2.jpg",
      "img3.jpg",
      "img4.jpg",
      "img5.jpg",
      "img6.jpg",
      "img7.jpg",
      "img8.jpg",
    ],
    c1: undefined,
    c2: undefined,
  }),
  methods: {
    handleResize() {
      if (window.innerWidth < 686) {
        this.numberOfSlides = 6;
      }
      if (window.innerWidth > 686) {
        this.numberOfSlides = 7;
      }
      if (window.innerWidth < 600) {
        this.numberOfSlides = 5;
      }
      if (window.innerWidth > 600 && window.innerWidth < 686) {
        this.numberOfSlides = 6;
      }
      if (window.innerWidth < 504) {
        this.numberOfSlides = 4;
      }
      if (window.innerWidth > 504 && window.innerWidth < 600) {
        this.numberOfSlides = 5;
      }
      if (window.innerWidth < 408) {
        this.numberOfSlides = 3;
      }
      if (window.innerWidth > 408 && window.innerWidth < 504) {
        this.numberOfSlides = 4;
      }
    },
    openFullscreen() {
      let image = event.target.nextSibling;
      let imageDiv = document.querySelector(".fullscreen-image");
      let newImage = document.querySelector(".new-image");
      newImage.src = image.src;
      imageDiv.style.display = "block";
    },
    hideMagnifier() {
      this.showMagnifier = false;
      setTimeout(() => {
        this.showMagnifier = true;
      }, 800);
    },
    closeFullscreen() {
      let imageDiv = document.querySelector(".fullscreen-image");
      imageDiv.style.display = "none";
    },
  },
  mounted() {
    this.c1 = this.$refs.c1;
    this.c2 = this.$refs.c2;
    if (window.innerWidth < 686) {
      this.numberOfSlides = 6;
    }
    if (window.innerWidth > 686) {
      this.numberOfSlides = 7;
    }
    if (window.innerWidth < 600) {
      this.numberOfSlides = 5;
    }
    if (window.innerWidth > 600 && window.innerWidth < 686) {
      this.numberOfSlides = 6;
    }
    if (window.innerWidth < 504) {
      this.numberOfSlides = 4;
    }
    if (window.innerWidth > 504 && window.innerWidth < 600) {
      this.numberOfSlides = 5;
    }
    if (window.innerWidth < 408) {
      this.numberOfSlides = 3;
    }
    if (window.innerWidth > 408 && window.innerWidth < 504) {
      this.numberOfSlides = 4;
    }
  },
  components: {
    VueSlickCarousel,
  },
  created() {
    window.addEventListener("resize", this.handleResize);
  },
  destroyed() {
    window.removeEventListener("resize", this.handleResize);
  },
};
</script>
