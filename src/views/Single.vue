<template>
  <div>
    <Header />
    <div class="wrapper">
      <div class="banner"></div>
      <div class="image-heading">
        <img src="../assets/SingleImg.png" alt="" />
        <img class="white-gradient" src="../assets/white-gradient.png" alt="" />
        <div class="text-heading">
          <p class="single-date">August 26, 2013</p>
          <p class="single-heading">
            'Margot' breathlessly reimagines Anne Frank's sister
          </p>
        </div>
      </div>
      <div class="main">
        <SingleNews />
        <SideContent />
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
import Header from "../components/Header";
import SideContent from "../components/SideContent";
import Footer from "../components/Footer";
import SingleNews from "../components/SingleNews";

export default {
  name: "Single",
  components: {
    Header,
    SingleNews,
    SideContent,
    Footer,
  },
};
</script>
