<template>
  <div class="side-content">
    <Sidebar />
    <Social />
  </div>
</template>

<script>
import Sidebar from "./Sidebar";
import Social from "./Social";

export default {
  components: {
    Sidebar,
    Social,
  },
  name: "SideContent",
};
</script>
