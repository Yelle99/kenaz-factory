<template>
  <div class="slider-img">
    <div class="gradient">
      <div class="text">
        <div class="top-text">
          <span class="date">{{ sliderNews.date }}</span>
          <img class="comment" src="../assets/comment.svg" alt="" />
          <span> {{ sliderNews.comments }}</span>
        </div>
        <h1 class="slider-heading">{{ sliderNews.heading }}</h1>
      </div>
      <router-link to="/single" tag="button">Read Article</router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: "SingleSliderNews",
  props: {
    sliderNews: Object,
  },
};
</script>
