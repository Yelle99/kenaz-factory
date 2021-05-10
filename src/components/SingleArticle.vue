<template>
  <a href="#" class="news-article">
    <img class="news-image" :src="require(`../assets/${newsdata.image}`)" />
    <div class="business-text">
      <p class="news-date">{{ newsdata.date }}</p>
      <h3 class="news-heading">
        {{ newsdata.heading }}
      </h3>
    </div>
  </a>
</template>

<script>
export default {
  name: "SingleArticle",
  props: {
    newsdata: Object,
  },
};
</script>
