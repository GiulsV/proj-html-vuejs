<template>
  <div class="container">
    <div class="text-center">
      <h2>Artist coaching</h2>
      <h3>Latest Online Courses</h3>
    </div>

    <div class="row d-flex justify-content-center" >
      <div class="col" v-for="(link, index) in courseCards" :key="index" id="ms_corsi">
        <div class="card h-100 border-0">
          <img class="card-img-top rounded-0" :src="link.img" :alt="link.alt" />
          <div class="card-body ms_card_body">
            <p class="card-text">
              {{ link.price }}
            </p>
            <p class="card-title mt-3">{{ link.title }}</p>

            <p class="card-text">
              <small class="text-muted">{{ link.text }}</small>
            </p>
          </div>
        </div>
      </div>
    </div>
    <div class="d-flex justify-content-center">
        <a class="btn bt_red" href="#" role="button">Get Started <i class="fa-solid fa-arrow-right"></i></a> 
    </div>
    
  </div>
</template>

<script>
export default {
  name: "CourseComp",
  data() {
    return {
      courseCards: [
        {
          img: require("@/assets/images/Corsi/artist-course-01-480x480.jpg"),
          alt: "corso",
          price: "$18.00",
          title: "The Acrylic Painting Academy",
          text: "",
        },
        {
          img: require("@/assets/images/Corsi/artist-course-02-480x480.jpg"),
          alt: "corso",
          price: "$21.00",
          title: "Drawing and Shading:Complete Course",
          text: "",
        },
        {
          img: require("@/assets/images/Corsi/artist-course-03-480x480.jpg"),
          alt: "corso",
          price: "$19.00",
          title: "The Color Theory for Digital Artist",
          text: "",
        },
        {
          img: require("@/assets/images/Corsi/artist-course-04-480x480.jpg"),
          alt: "corso",
          price: "$35.00",
          title: "Ultimate Guide To Digital Sketching for Beginner",
          text: "",
        },
        {
          img: require("@/assets/images/Corsi/artist-course-05-480x480.jpg"),
          alt: "corso",
          price: "$19.00",
          title: "Portrait Drawing The Smart Way",
          text: "",
        },
        {
          img: require("@/assets/images/Corsi/artist-course-06-480x480.jpg"),
          alt: "corso",
          price: "$19.00",
          title: "Mastering Watercolor Painting from Beginner",
          text: "",
        },
        {
          img: require("@/assets/images/Corsi/artist-course-07-480x480.jpg"),
          alt: "corso",
          price: "$25.00",
          title: "The art & Scince of Drawing",
          text: "",
        },
        {
          img: require("@/assets/images/Corsi/artist-course-08-480x480.jpg"),
          alt: "corso",
          price: "$22.00",
          title: "The Colored Pencil Drawing Course",
          text: "",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
#ms_corsi{
    flex-basis: calc(100% / 4);
}
.ms_card_body{
    width: 80%;
    &:hover{
        transform: translateY(-25px);
        background-color: white;
        border: 2px solid orange;
    }
}

img{
  width: 95%;
}
</style>
