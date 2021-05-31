<template>
  <section>
    <h1 class="footernews-heading">{{ footerHeading }}</h1>
    <div class="footer-news">
      <article
        class="footer-article"
        :key="footerNews.id"
        v-for="footerNews in footerNews"
      >
        <div class="footer-text">
          <p class="footer-date">{{ footerNews.date }}</p>
          <p class="footer-num">{{ footerNews.num }}</p>
          <h3 class="footer-heading">{{ footerNews.heading }}</h3>
        </div>
        <img
          class="footer-img"
          :src="require(`../assets/${footerNews.image}`)"
          alt=""
        />
      </article>
    </div>
  </section>
</template>

<script>
export default {
  name: "FooterNews",
  props: {
    footerHeading: String,
    newsType: String,
  },
  data() {
    return {
      footerNews: [],
    };
  },
  methods: {
    getFooterData(category) {
      if (category == "featured") {
        this.footerNews = [
          {
            id: 1,
            image: "footerimage.png",
            date: "August 26, 2013",
            heading: "Palestinians call off peace talks after clash",
            num: "5",
          },
          {
            id: 2,
            image: "footerimage.png",
            date: "August 26, 2013",
            heading: "Palestinians call off peace talks after clash",
            num: "5",
          },
          {
            id: 3,
            image: "footerimage.png",
            date: "August 26, 2013",
            heading: "Palestinians call off peace talks after clash",
            num: "5",
          },
        ];
      }
      if (category == "randomposts") {
        this.footerNews = [
          {
            id: 1,
            image: "footerimage.png",
            date: "August 26, 2013",
            heading: "Palestinians call off peace talks after clash",
            num: "5",
          },
          {
            id: 2,
            image: "footerimage.png",
            date: "August 26, 2013",
            heading: "Palestinians call off peace talks after clash",
            num: "5",
          },
          {
            id: 3,
            image: "footerimage.png",
            date: "August 26, 2013",
            heading: "Palestinians call off peace talks after clash",
            num: "5",
          },
        ];
      }
    },
  },
  beforeMount() {
    this.getFooterData(this.newsType);
  },
};
</script>
