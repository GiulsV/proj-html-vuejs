<template>
  <div class="container">
    <div class="text-center">
      <h2>Articles and Tips</h2>
      <h3>Latest from the Blog</h3>
    </div>

    <div class="row d-flex justify-content-center" >
      <div class="col" v-for="(link, index) in blogCards" :key="index" id="ms_corsi">
        <div class="card">
          <img class="card-img-top rounded-0" :src="link.img" :alt="link.alt" />
          <div class="card-body ms_card_body">
            <p class="card-text">
              {{ link.tag}}
            </p>
            <p class="card-title mt-3">{{ link.title }}</p>

            <p class="card-text">
              <small class="text-muted"><i class="far fa-calendar"></i>{{ link.date}} <i class="far fa-eye"></i>{{link.views}}</small>
            </p>
          </div>
        </div>
      </div>
    </div>

    
  </div>
</template>

<script>
export default {
  name: "BlogComp",
  data() {
    return {
      blogCards: [
        {
          img: require("@/assets/images/blog/artist-blog-03-480x356.jpeg"),
          alt: "blog",
          tag: "ARTIST",
          title: "Brush Strokes Energize Trees in Paintings",
          date:"15 May, 2020",
          views: "364",
        },
        {
          img: require("@/assets/images/blog/artist-blog-02-500x680.jpg"),
          alt: "blog",
          tag: "ARTIST",
          title: "Connection Between Self-Portraits and Identity",
          date:"15 May, 2020",
          views: "364",
        },
        {
          img: require("@/assets/images/blog/artist-blog-01-480x356.jpg"),
          alt: "blog",
          tag: "ARTIST",
          title: "Pocket-Sized Notebooks Hold Miniature Paintings",
          date:"15 May, 2020",
          views: "364",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style/_commons.scss";
@import "../assets/style/_variables.scss";
</style>