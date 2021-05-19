<template>
  <router-link to="/single" tag="article" class="sidebar-article">
    <div class="sidebar-text">
      <p class="sidebar-comments">
        <img class="comment" src="../assets/comment.svg" alt="" />{{
          sidebarNews.comments
        }}
      </p>
      <p class="sidebar-date">{{ sidebarNews.date }}</p>
      <h3 class="sidebar-heading">
        {{ sidebarNews.heading }}
      </h3>
    </div>
    <img class="sidebar-img" :src="require(`../assets/${sidebarNews.image}`)" />
  </router-link>
</template>

<script>
export default {
  name: "SidebarArticle",
  props: {
    sidebarNews: Object,
  },
};
</script>
