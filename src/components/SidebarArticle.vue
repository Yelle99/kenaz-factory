<template>
  <a href="#" class="sidebar-article">
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
  </a>
</template>

<script>
export default {
  name: "SidebarArticle",
  props: {
    sidebarNews: Object,
  },
};
</script>
