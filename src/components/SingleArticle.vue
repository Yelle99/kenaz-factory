<template>
  <router-link to="/single" tag="article" class="news-article">
    <img class="news-image" :src="require(`../assets/${newsData.image}`)" />
    <div class="business-text">
      <span class="news-date">{{ newsData.date }}</span>
      <span class="news-num">{{ newsData.num }}</span>
      <h3 class="news-heading">
        {{ newsData.heading }}
      </h3>
    </div>
  </router-link>
</template>

<script>
export default {
  name: "SingleArticle",
  props: {
    newsData: Object,
  },
};
</script>
