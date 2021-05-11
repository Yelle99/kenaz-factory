<template>
  <div class="side-content">
    <Sidebar />
    <Social />
    <KenazTV />
    <div class="side-banners">
      <div class="side-banner"></div>
      <div class="side-banner"></div>
    </div>
    <div class="facebook-banner"></div>
  </div>
</template>

<script>
import Sidebar from "./Sidebar";
import Social from "./Social";
import KenazTV from "./KenazTV";

export default {
  components: {
    Sidebar,
    Social,
    KenazTV,
  },
  name: "SideContent",
};
</script>
