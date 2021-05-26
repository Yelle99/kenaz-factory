<template>
  <section
    :class="[
      border,
      isDouble ? 'carouselsection-double' : 'carouselsection-single',
    ]"
  >
    <h1>{{ title }}</h1>
    <VueSlickCarousel
      :slidesToShow="isDouble && windowSize ? 2 : 1"
      :dots="false"
      :arrows="true"
    >
      <div
        class="carousel-news"
        :key="singleCarouselnews.id"
        v-for="singleCarouselnews in carouselnews"
      >
        <SingleArticle :newsdata="singleCarouselnews" />
      </div>
      <template #prevArrow="arrowOption">
        <div class="prev-arrow">
          {{ arrowOption.currentSlide }}/{{ arrowOption.slideCount }}
        </div>
      </template>
      <template #nextArrow="arrowOption">
        <div class="next-arrow">
          {{ arrowOption.currentSlide }}/{{ arrowOption.slideCount }}
        </div>
      </template>
    </VueSlickCarousel>
  </section>
</template>

<script>
import SingleArticle from "./SingleArticle";
import VueSlickCarousel from "vue-slick-carousel";
import "vue-slick-carousel/dist/vue-slick-carousel.css";

export default {
  name: "CarouselSection",
  components: {
    VueSlickCarousel,
    SingleArticle,
  },
  props: {
    border: String,
    isDouble: Boolean,
    newsType: String,
    title: String,
  },
  data() {
    return {
      windowSize: true,
      carouselnews: [],
    };
  },
  methods: {
    handleResize() {
      if (window.innerWidth < 640) {
        this.windowSize = false;
      }
      if (window.innerWidth > 640) {
        this.windowSize = true;
      }
    },
    getData(category) {
      if (category == "carouselnews") {
        this.carouselnews = [
          {
            id: 1,
            image: "newsimage.png",
            date: "August 26, 2013",
            heading: "For Obama, MLK's shadow looms large ahead of speech",
          },
          {
            id: 2,
            image: "newsimage.png",
            date: "August 26, 2013",
            heading: "NASA releases portrait of a planet waving at Saturn",
          },
          {
            id: 3,
            image: "newsimage.png",
            date: "August 26, 2013",
            heading: "Patriotsvv make cuts... and Tim Tebow survives (so far)",
          },
          {
            id: 4,
            image: "newsimage.png",
            date: "August 26, 2013",
            heading: "Palestinians call off peace talks after clash",
          },
        ];
      }
      if (category == "editorials") {
        this.carouselnews = [
          {
            id: 1,
            image: "newsimage.png",
            date: "August 26, 2013",
            heading: "For Obama, MLK's shadow looms large ahead of speech",
          },
          {
            id: 2,
            image: "newsimage.png",
            date: "August 26, 2013",
            heading: "NASA releases portrait of a planet waving at Saturn",
          },
          {
            id: 3,
            image: "newsimage.png",
            date: "August 26, 2013",
            heading: "Patriotsvv make cuts... and Tim Tebow survives (so far)",
          },
          {
            id: 4,
            image: "newsimage.png",
            date: "August 26, 2013",
            heading: "Palestinians call off peace talks after clash",
          },
        ];
      }
      if (category == "localnews") {
        this.carouselnews = [
          {
            id: 1,
            image: "newsimage.png",
            date: "August 26, 2013",
            heading: "For Obama, MLK's shadow looms large ahead of speech",
          },
          {
            id: 2,
            image: "newsimage.png",
            date: "August 26, 2013",
            heading: "NASA releases portrait of a planet waving at Saturn",
          },
          {
            id: 3,
            image: "newsimage.png",
            date: "August 26, 2013",
            heading: "Patriotsvv make cuts... and Tim Tebow survives (so far)",
          },
          {
            id: 4,
            image: "newsimage.png",
            date: "August 26, 2013",
            heading: "Palestinians call off peace talks after clash",
          },
        ];
      }
    },
  },
  beforeMount() {
    this.getData(this.newsType);
  },
  created() {
    window.addEventListener("resize", this.handleResize);
  },
  destroyed() {
    window.removeEventListener("resize", this.handleResize);
  },
  mounted() {
    if (window.innerWidth < 640) {
      this.windowSize = false;
    }
    if (window.innerWidth > 640) {
      this.windowSize = true;
    }
  },
};
</script>
