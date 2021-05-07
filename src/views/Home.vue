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
        <div class="side-content">
          <Sidebar />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Header from "../components/Header";
import Slider from "../components/Slider";
import CategorySection from "../components/CategorySection";
import Sidebar from "../components/Sidebar";

export default {
  name: "Home",
  components: {
    Header,
    Slider,
    CategorySection,
    Sidebar,
  },
};
</script>
