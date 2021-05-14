<template>
  <section>
    <h1 class="footernews-heading">{{ footerHeading }}</h1>
    <div class="footer-news">
      <article
        class="footer-article"
        :key="footernews.id"
        v-for="footernews in footernews"
      >
        <div class="footer-text">
          <p class="footer-date">{{ footernews.date }}</p>
          <p class="footer-num">{{ footernews.num }}</p>
          <h3 class="footer-heading">{{ footernews.heading }}</h3>
        </div>
        <img
          class="footer-img"
          :src="require(`../assets/${footernews.image}`)"
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
      footernews: [],
    };
  },
  methods: {
    getFooterData(category) {
      if (category == "featured") {
        this.footernews = [
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
        this.footernews = [
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
