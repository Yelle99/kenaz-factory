<template>
  <a href="#" class="news-article">
    <img class="news-image" :src="require(`../assets/${newsdata.image}`)" />
    <div class="business-text">
      <span class="news-date">{{ newsdata.date }}</span>
      <span class="news-num">{{ newsdata.num }}</span>
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
