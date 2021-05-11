<template>
  <aside class="tv">
    <h1>Kenaz TV</h1>
    <iframe
      width="300"
      height="149"
      :src="videosrc"
      title="YouTube video player"
      frameborder="0"
      allowfullscreen
    ></iframe>
    <div class="tv-text">
      <p class="tv-date">{{ date }}</p>
      <h3 class="tv-heading">{{ heading }}</h3>
    </div>
  </aside>
</template>

<script>
export default {
  name: "KenazTV",
  data() {
    return {
      videosrc: "https://www.youtube.com/embed/l6veMGLpol0",
      date: "August 26, 2013",
      heading: "NASA releases portrait of a planet waving at Saturn",
    };
  },
};
</script>
