<template>
  <div class="wrapper">
    <div class="container">

 
    <div class="text-center ms_padding_title">
      <h2>Artist coaching</h2>
      <h4>Latest Online Courses</h4>
    </div>

    <div class="row d-flex justify-content-center ms_padding_title" >
      <div class="col pb-5" v-for="(link, index) in courseCards" :key="index" id="ms_corsi">
        <div class="card  border-0">
          <img class="card-img-top  rounded-0" :src="link.img" :alt="link.alt" />
          <div class="card-body ms_card_body">
            <p class="card-text ms_color-text">
              {{ link.price }}
            </p>
            <h6 class="card-title mt-3">{{ link.title }}</h6>

            <div class="card-footer bg-transparent p-0 border-0 align-items-end">
              <small class="text-muted"><i class="far fa-file-alt"></i> {{ link.text }} Lesson</small>
              <small class="text-muted"><i class="fas fa-user"></i> {{link.student}} Student</small>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="d-flex justify-content-center">
        <a class="btn bt_red" href="#" role="button">Get Started <i class="fa-solid fa-arrow-right"></i></a> 
    </div>
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
          text: "4",
          student:"50",
        },
        {
          img: require("@/assets/images/Corsi/artist-course-02-480x480.jpg"),
          alt: "corso",
          price: "$21.00",
          title: "Drawing and Shading:Complete Course",
          text: "14",
          student:"50",
        },
        {
          img: require("@/assets/images/Corsi/artist-course-03-480x480.jpg"),
          alt: "corso",
          price: "$19.00",
          title: "The Color Theory for Digital Artist",
          text: "7",
          student:"50",
        },
        {
          img: require("@/assets/images/Corsi/artist-course-04-480x480.jpg"),
          alt: "corso",
          price: "$35.00",
          title: "Ultimate Guide To Digital Sketching for Beginner",
          text: "4",
          student:"50",
        },
        {
          img: require("@/assets/images/Corsi/artist-course-05-480x480.jpg"),
          alt: "corso",
          price: "$19.00",
          title: "Portrait Drawing The Smart Way",
          text: "20",
          student:"50",
        },
        {
          img: require("@/assets/images/Corsi/artist-course-06-480x480.jpg"),
          alt: "corso",
          price: "$19.00",
          title: "Mastering Watercolor Painting from Beginner",
          text: "4",
          student:"50",
        },
        {
          img: require("@/assets/images/Corsi/artist-course-07-480x480.jpg"),
          alt: "corso",
          price: "$25.00",
          title: "The art & Science of Drawing",
          text: "9",
          student:"50",
        },
        {
          img: require("@/assets/images/Corsi/artist-course-08-480x480.jpg"),
          alt: "corso",
          price: "$22.00",
          title: "The Colored Pencil Drawing Course",
          text: "2",
          student:"50",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style/_commons.scss";
@import "../assets/style/_variables.scss";
h2{
  color:$Cerulean;
  font-family: 'Satisfy', cursive;
}
h4{
  font-weight: bold;
}
#ms_corsi{
    flex-basis: calc(100% / 4);
}
.ms_card_body{
    width: 85%;
    height: 175px;
    &:hover{
        transform: translateY(-30px);
        background-color: white;
        border: 2px solid orange;
    }
}
img{
  width: 100%;
}

.fa-arrow-right{
  margin-left: 0.2rem;
}

.fa-user{
  margin-left: 10px;
}
</style>
