<template>
  <div class="home">
    <Header />
    <div class="wrapper">
      <div class="banner"></div>
      <Slider />
      <div class="main">
        <div class="categories">
          <CategorySection border="news-border" title="News" />
          <CategorySection border="sport-border" title="Sports" />
          <div class="banner-news"></div>
        </div>
        <SideContent />
      </div>
    </div>
  </div>
</template>

<script>
import Header from "../components/Header";
import Slider from "../components/Slider";
import SideContent from "../components/SideContent";
import CategorySection from "../components/CategorySection";

export default {
  name: "Home",
  components: {
    Header,
    Slider,
    CategorySection,
    SideContent,
  },
};
</script>
