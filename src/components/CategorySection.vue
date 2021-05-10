<template>
  <section>
    <div :class="['category', border]">
      <div class="heading">
        <h1>{{ title }}</h1>
        <a href="#">See all</a>
      </div>
      <div v-if="isNews == true" class="news">
        <div :key="news.id" v-for="news in allnews">
          <SingleArticle :newsdata="news" />
        </div>
      </div>
      <div v-if="isSports == true" class="sports">
        <div :key="sport.id" v-for="sport in sports">
          <SingleArticle :newsdata="sport" />
        </div>
      </div>
      <div v-if="isBusiness == true" class="business">
        <div :key="business.id" v-for="business in business">
          <SingleArticle :newsdata="business" />
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
    isSports: Boolean,
    isNews: Boolean,
    isBusiness: Boolean,
  },
  data() {
    return {
      allnews: [
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
          heading: "Patriotsvv make cuts... and Tim Tebrov survives (so far)",
        },
      ],
      sports: [
        {
          id: 4,
          image: "newsimage.png",
          date: "August 26, 2013",
          heading: "For Obama, MLK's shadow looms large ahead of speech",
        },
        {
          id: 5,
          image: "newsimage.png",
          date: "August 26, 2013",
          heading: "NASA releases portrait of a planet waving at Saturn",
        },
        {
          id: 6,
          image: "newsimage.png",
          date: "August 26, 2013",
          heading: "Patriotsvv make cuts... and Tim Tebrov survives (so far)",
        },
      ],
      business: [
        {
          id: 7,
          image: "newsimage.png",
          date: "August 26, 2013",
          heading: "For Obama, MLK's shadow looms large ahead of speech",
        },
        {
          id: 8,
          image: "newsimage.png",
          date: "August 26, 2013",
          heading: "For Obama, MLK's shadow looms large ahead of speech",
        },
        {
          id: 9,
          image: "newsimage.png",
          date: "August 26, 2013",
          heading: "For Obama, MLK's shadow looms large ahead of speech",
        },
        {
          id: 10,
          image: "newsimage.png",
          date: "August 26, 2013",
          heading: "For Obama, MLK's shadow looms large ahead of speech",
        },
      ],
    };
  },
};
</script>
