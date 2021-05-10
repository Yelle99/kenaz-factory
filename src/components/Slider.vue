<template>
  <div class="slider-container">
    <VueSlickCarousel :dots="false" :arrows="true">
      <div :key="sliderNews.id" v-for="sliderNews in sliderNews">
        <SingleSliderNews :sliderNews="sliderNews" />
      </div>
    </VueSlickCarousel>
  </div>
</template>

<script>
import SingleSliderNews from "./SingleSliderNews";
import VueSlickCarousel from "vue-slick-carousel";
import "vue-slick-carousel/dist/vue-slick-carousel.css";
// carousel custom style
import "vue-slick-carousel/dist/custom-theme.css";

export default {
  name: "Slider",
  components: {
    VueSlickCarousel,
    SingleSliderNews,
  },
  data() {
    return {
      sliderNews: [
        {
          id: 1,
          date: "August 26, 2013",
          comments: "22 comments",
          heading: "'Margot' breathlessly reimagines Anne Frank's sister",
        },
        {
          id: 2,
          date: "August 26, 2013",
          comments: "22 comments",
          heading: "'Margot' breathlessly reimagines Anne Frank's sister",
        },
        {
          id: 3,
          date: "August 26, 2013",
          comments: "22 comments",
          heading: "'Margot' breathlessly reimagines Anne Frank's sister",
        },
      ],
    };
  },
};
</script>
