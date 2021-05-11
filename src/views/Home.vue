<template>
  <div class="home">
    <Header />
    <div class="wrapper">
      <div class="banner"></div>
      <Slider />
      <div class="main">
        <div class="categories">
          <CategorySection border="news-border" title="News" :isNews="true" />
          <CategorySection
            border="sport-border"
            title="Sports"
            :isSports="true"
          />
          <div class="banner-news"></div>
          <CategorySection
            border="business-border"
            title="Business"
            :isBusiness="true"
          />
          <div class="banner-news"></div>
          <CarouselSection :isDouble="true" border="carousel-news-border" />
          <div class="single-carousels">
            <CarouselSection
              :isDouble="false"
              border="carousel-travel-border"
            />
            <CarouselSection
              :isDouble="false"
              border="carousel-travel-border"
            />
          </div>
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
import CarouselSection from "../components/CarouselSection";

export default {
  name: "Home",
  components: {
    Header,
    Slider,
    CategorySection,
    SideContent,
    CarouselSection,
  },
};
</script>
