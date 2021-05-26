<template>
  <div>
    <Header />
    <div class="wrapper">
      <div class="banner"></div>
      <Slider />
      <div class="main-categorypage">
        <News />
        <SideContent />
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
import Header from "../components/Header";
import Slider from "../components/Slider";
import News from "../components/News";
import SideContent from "../components/SideContent";
import Footer from "../components/Footer";

export default {
  name: "Category",
  components: {
    Header,
    Slider,
    News,
    SideContent,
    Footer,
  },
};
</script>
