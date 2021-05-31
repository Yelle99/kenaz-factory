<template>
  <article class="categorynews">
    <h3 class="categorynews-heading">
      {{ newsData.heading }}
    </h3>
    <div class="categorynews_top-text">
      <span class="categorynews-date">
        <img src="../assets/calendar.svg" alt="" />
        <p>{{ newsData.date }}</p>
      </span>
      <p class="categorynews-author">Author: {{ newsData.author }}</p>
      <p class="categorynews-comments">{{ newsData.comments }} comments</p>
    </div>
    <div class="categorynews-content">
      <img
        class="categorynews-image"
        :src="require(`../assets/${newsData.image}`)"
      />
      <p class="categorynews-text">{{ newsData.text }}</p>
    </div>
    <router-link to="/single" tag="button" class="read-article"
      >Read Article</router-link
    >
  </article>
</template>

<script>
export default {
  name: "NewsArticle",
  props: {
    newsData: Object,
  },
};
</script>
