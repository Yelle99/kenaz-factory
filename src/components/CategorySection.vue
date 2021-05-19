<template>
  <section :class="['category', border]">
    <div class="heading">
      <h1>{{ title }}</h1>
      <router-link to="/category">See all</router-link>
    </div>
    <div :class="[isBusiness ? 'business' : 'news']">
      <div :key="news.id" v-for="news in news">
        <SingleArticle :newsdata="news" />
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
    newsType: String,
    isBusiness: Boolean,
  },
  data() {
    return {
      news: [],
    };
  },
  methods: {
    getData(category) {
      if (category == "allnews") {
        this.news = [
          {
            id: 1,
            image: "newsimage.png",
            date: "August 26, 2013",
            heading: "For Obama, MLK's shadow looms large ahead of speech",
            num: "14",
          },
          {
            id: 2,
            image: "newsimage.png",
            date: "August 26, 2013",
            heading: "NASA releases portrait of a planet waving at Saturn",
            num: "22",
          },
          {
            id: 3,
            image: "newsimage.png",
            date: "August 26, 2013",
            heading: "Patriotsvv make cuts... and Tim Tebow survives (so far)",
            num: "5",
          },
        ];
      }
      if (category == "sport") {
        this.news = [
          {
            id: 1,
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
            heading: "Patriotsvv make cuts... and Tim Tebow survives (so far)",
          },
        ];
      }
      if (category == "business") {
        this.news = [
          {
            id: 1,
            image: "newsimage.png",
            date: "August 26, 2013",
            heading: "For Obama, MLK's shadow looms large ahead of speech",
          },
          {
            id: 2,
            image: "newsimage.png",
            date: "August 26, 2013",
            heading: "For Obama, MLK's shadow looms large ahead of speech",
          },
          {
            id: 3,
            image: "newsimage.png",
            date: "August 26, 2013",
            heading: "For Obama, MLK's shadow looms large ahead of speech",
          },
          {
            id: 4,
            image: "newsimage.png",
            date: "August 26, 2013",
            heading: "For Obama, MLK's shadow looms large ahead of speech",
          },
        ];
      }
    },
  },
  beforeMount() {
    this.getData(this.newsType);
  },
};
</script>
