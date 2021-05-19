<template>
  <article class="categorynews">
    <h3 class="categorynews-heading">
      {{ newsdata.heading }}
    </h3>
    <div class="categorynews_top-text">
      <span class="categorynews-date">
        <img src="../assets/calendar.svg" alt="" />
        <p>{{ newsdata.date }}</p>
      </span>
      <p class="categorynews-author">Author: {{ newsdata.author }}</p>
      <p class="categorynews-comments">{{ newsdata.comments }} comments</p>
    </div>
    <div class="categorynews-content">
      <img
        class="categorynews-image"
        :src="require(`../assets/${newsdata.image}`)"
      />
      <p class="categorynews-text">{{ newsdata.text }}</p>
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
    newsdata: Object,
  },
};
</script>
