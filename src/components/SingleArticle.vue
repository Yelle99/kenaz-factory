<template>
  <article>
    <img class="news-image" :src="require(`../assets/${news.image}`)" />
    <p class="news-date">{{ news.date }}</p>
    <h3 class="news-heading">
      {{ news.heading }}
    </h3>
  </article>
</template>

<script>
export default {
  name: "SingleArticle",
  props: {
    news: Object,
  },
};
</script>
