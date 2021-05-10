<template>
  <aside class="sidebar">
    <div class="btns">
      <button class="active">Popular</button>
      <button>Top Rated</button>
      <button>Comments</button>
    </div>
    <div class="sidebar-news">
      <article
        class="article-container"
        :key="sidebarNews.id"
        v-for="sidebarNews in sidebarNews"
      >
        <SidebarArticle :sidebarNews="sidebarNews" />
      </article>
    </div>
  </aside>
</template>

<script>
import SidebarArticle from "./SidebarArticle";

export default {
  name: "Sidebar",
  components: {
    SidebarArticle,
  },
  data() {
    return {
      sidebarNews: [
        {
          id: 1,
          comments: 5,
          image: "sidebarnewsimage.png",
          date: "August 26, 2013",
          heading: "Palestinians call off peace talks after clash",
        },
        {
          id: 2,
          comments: 5,
          image: "sidebarnewsimage.png",
          date: "August 26, 2013",
          heading: "Palestinians call off peace talks after clash",
        },
        {
          id: 3,
          comments: 5,
          image: "sidebarnewsimage.png",
          date: "August 26, 2013",
          heading: "Palestinians call off peace talks after clash",
        },
        {
          id: 4,
          comments: 5,
          image: "sidebarnewsimage.png",
          date: "August 26, 2013",
          heading: "Palestinians call off peace talks after clash",
        },
        {
          id: 5,
          comments: 5,
          image: "sidebarnewsimage.png",
          date: "August 26, 2013",
          heading: "Palestinians call off peace talks after clash",
        },
      ],
    };
  },
};
</script>
