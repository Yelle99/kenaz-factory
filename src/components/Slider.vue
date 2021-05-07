<template>
  <div class="slider-container">
    <VueSlickCarousel :dots="false" :arrows="true">
      <div class="slider-img">
        <div class="gradient">
          <div class="text">
            <div class="top-text">
              <span class="date">August 26, 2013 </span>
              <img class="comment" src="../assets/comment.svg" alt="" />
              <span> 22 comments</span>
            </div>
            <h1>'Margot' breathlessly reimagines Anne Frank's sister</h1>
          </div>
          <button>Read Article</button>
        </div>
      </div>
      <div class="slider-img">
        <div class="gradient">
          <div class="text">
            <div class="top-text">
              <span class="date">August 26, 2013 </span>
              <img class="comment" src="../assets/comment.svg" alt="" />
              <span> 22 comments</span>
            </div>
            <h1>'Margot' breathlessly reimagines Anne Frank's sister</h1>
          </div>
          <button>Read Article</button>
        </div>
      </div>
      <div class="slider-img">
        <div class="gradient">
          <div class="text">
            <div class="top-text">
              <span class="date">August 26, 2013 </span>
              <img class="comment" src="../assets/comment.svg" alt="" />
              <span> 22 comments</span>
            </div>
            <h1>'Margot' breathlessly reimagines Anne Frank's sister</h1>
          </div>
          <button>Read Article</button>
        </div>
      </div>
    </VueSlickCarousel>
  </div>
</template>

<script>
import VueSlickCarousel from "vue-slick-carousel";
import "vue-slick-carousel/dist/vue-slick-carousel.css";
// carousel custom style
import "vue-slick-carousel/dist/custom-theme.css";

export default {
  name: "Slider",
  components: {
    VueSlickCarousel,
  },
};
</script>
