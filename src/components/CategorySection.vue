<template>
  <section>
    <div :class="['category', border]">
      <div class="heading">
        <h1>{{ title }}</h1>
        <a href="#">See all</a>
      </div>
      <div class="news">
        <div :key="news.id" v-for="news in news">
          <SingleArticle :news="news" />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import SingleArticle from "./SingleArticle";

export default {
  name: "CategorySection",
  components: {
    SingleArticle,
  },
  props: {
    title: String,
    border: String,
  },
  data() {
    return {
      news: [
        {
          id: 1,
          // image: "/img/newsimage.53bca389.png",
          image: "newsimage.png",
          date: "August 26, 2013",
          heading: "For Obama, MLK's shadow looms large ahead of speech",
        },
        {
          id: 2,
          image: "newsimage.png",
          date: "August 26, 2013",
          heading: "NASA releases portrait of a planet waving at Saturn",
        },
        {
          id: 3,
          image: "newsimage.png",
          date: "August 26, 2013",
          heading: "Patriotsvv make cuts... and Tim Tebrov survives (so far)",
        },
      ],
    };
  },
};
</script>
