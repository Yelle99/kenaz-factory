<template>
  <div>
    <section class="all-news">
      <h1>News</h1>
      <div :key="categoryNews.id" v-for="categoryNews in categoryNews">
        <NewsArticle :newsdata="categoryNews" />
      </div>
      <div class="pages">
        <button class="selected">1</button>
        <button>2</button>
        <button>3</button>
        <button>4</button>
        <button>5</button>
        <button>6</button>
        <button>7</button>
        <button>8</button>
        <button>9</button>
        <button>10</button>
      </div>
    </section>
    <div class="banner-news"></div>
  </div>
</template>

<script>
import NewsArticle from "./NewsArticle";

export default {
  name: "News",
  components: {
    NewsArticle,
  },
  data() {
    return {
      categoryNews: [
        {
          id: 1,
          image: "newsimage.png",
          date: "August 26, 2013",
          heading: "Patriotsvv make cuts... and Tim Tebow survives (so far)",
          author: "Matej Sudar",
          comments: "12",
          text:
            "Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo. ",
        },
        {
          id: 2,
          image: "newsimage.png",
          date: "August 26, 2013",
          heading: "Patriotsvv make cuts... and Tim Tebow survives (so far)",
          author: "Matej Sudar",
          comments: "12",
          text:
            "Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo. ",
        },
        {
          id: 3,
          image: "newsimage.png",
          date: "August 26, 2013",
          heading: "Patriotsvv make cuts... and Tim Tebow survives (so far)",
          author: "Matej Sudar",
          comments: "12",
          text:
            "Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo. ",
        },
        {
          id: 4,
          image: "newsimage.png",
          date: "August 26, 2013",
          heading: "Patriotsvv make cuts... and Tim Tebow survives (so far)",
          author: "Matej Sudar",
          comments: "12",
          text:
            "Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo. ",
        },
        {
          id: 5,
          image: "newsimage.png",
          date: "August 26, 2013",
          heading: "Patriotsvv make cuts... and Tim Tebow survives (so far)",
          author: "Matej Sudar",
          comments: "12",
          text:
            "Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo. ",
        },
        {
          id: 6,
          image: "newsimage.png",
          date: "August 26, 2013",
          heading: "Patriotsvv make cuts... and Tim Tebow survives (so far)",
          author: "Matej Sudar",
          comments: "12",
          text:
            "Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo. ",
        },
      ],
    };
  },
};
</script>
