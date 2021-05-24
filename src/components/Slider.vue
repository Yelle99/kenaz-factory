<template>
  <div class="slider-container">
    <VueSlickCarousel :dots="false" :arrows="true">
      <div :key="singleSliderNews.id" v-for="singleSliderNews in sliderNews">
        <SingleSliderNews :sliderNews="singleSliderNews" />
      </div>
      <template #prevArrow="arrowOption">
        <div class="prev-arrow-slider">
          {{ arrowOption.currentSlide }}/{{ arrowOption.slideCount }}
        </div>
      </template>
      <template #nextArrow="arrowOption">
        <div class="next-arrow-slider">
          {{ arrowOption.currentSlide }}/{{ arrowOption.slideCount }}
        </div>
      </template>
    </VueSlickCarousel>
  </div>
</template>

<script>
import SingleSliderNews from "./SingleSliderNews";
import VueSlickCarousel from "vue-slick-carousel";

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
