<template>
  <div class="home">
    <Header />
    <Slider />
    <CategorySection :title="News" />
  </div>
</template>

<script>
import Header from "../components/Header";
import Slider from "../components/Slider";
import CategorySection from "../components/CategorySection";

export default {
  name: "Home",
  components: {
    Header,
    Slider,
    CategorySection,
  },
};
</script>
