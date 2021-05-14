<template>
  <div class="home">
    <Header />
    <div class="wrapper">
      <div class="banner"></div>
      <Slider />
      <div class="main">
        <div class="categories">
          <CategorySection
            border="news-border"
            title="News"
            newsType="allnews"
          />
          <CategorySection
            border="sport-border"
            title="Sport"
            newsType="sport"
          />
          <div class="banner-news"></div>
          <CategorySection
            border="business-border"
            title="Business"
            newsType="business"
            :isBusiness="true"
          />
          <div class="banner-news"></div>
          <CarouselSection
            title="News Carousel"
            :isDouble="true"
            border="carousel-news-border"
            newsType="carouselnews"
          />
          <div class="single-carousels">
            <CarouselSection
              title="Editorials"
              :isDouble="false"
              border="carousel-travel-border"
              newsType="editorials"
            />
            <CarouselSection
              title="Local News"
              :isDouble="false"
              border="carousel-travel-border"
              newsType="localnews"
            />
          </div>
        </div>
        <SideContent />
      </div>
      <div class="banner"></div>
      <ImageCarousel />
    </div>
    <Footer />
  </div>
</template>

<script>
import Header from "../components/Header";
import Slider from "../components/Slider";
import SideContent from "../components/SideContent";
import CategorySection from "../components/CategorySection";
import CarouselSection from "../components/CarouselSection";
import ImageCarousel from "../components/ImageCarousel";
import Footer from "../components/Footer";

export default {
  name: "Home",
  components: {
    Header,
    Slider,
    CategorySection,
    SideContent,
    CarouselSection,
    ImageCarousel,
    Footer,
  },
};
</script>
