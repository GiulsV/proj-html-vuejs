<template>
  <div class="container" id="ms_card">
    <div class="text-center ms_padding_title">
      <h2>Articles and Tips</h2>
      <h4>Latest from the Blog</h4>
    </div>

    <div class="row d-flex justify-content-center " >
      <div class="col ms_card_blog" v-for="(link, index) in blogCards" :key="index">
        <div class="card border-0  " >
          <img class="card-img-top rounded-0" :src="link.img" :alt="link.alt" />
          <div class="card-body ">
            <small class="card-text text-muted">
              {{ link.tag}}
            </small>
            <p class="card-title mt-3">{{ link.title }}</p>

            <p class="card-text">
              <small class="text-muted">
                <i class="far fa-calendar"></i>{{ link.date}} 
                <i class="far fa-eye"></i>{{link.views}}
              </small>
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
#ms_card{
  background-image: url("@/assets/images/Sagome/maxcoach-shape-05.png");
  background-repeat: no-repeat;
  background-position: top 17% right 63%;
}

h2{
  color:$Cerulean;
  font-family: 'Satisfy', cursive;
}
h4{
  font-weight: bold;
}
.ms_card_blog:first-child{
  margin-top: 13%;
}
.ms_card_blog:last-child{
  margin-top: 5%;
}
i{
  margin: 5px 5px;
}
</style>