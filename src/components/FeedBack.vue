<template>
  <div class="container-fluid d-flex flex-column">
    <div class="text-center ms_padding_title">
    <h2>Testimonials</h2>
    <h4>Why do people love me?</h4>
    </div>

    <div class="d-flex">
    <div class="card rounded-0 border-0 mx-4 px-3 ms_opacity" v-for="(link, i) in feedBackList" :key="i">
      <div class="card-body">
        <h6 class="card-title fw-bold">{{link.title}}</h6>
        <p class="card-text text-muted fs-6">
            {{link.text}}
        </p>

      </div>
      <div class="card-img-bottom px-3 pb-5 d-flex">
      <img :src="link.img" :alt="link.alt" class="rounded-circle"/>
      <p class="card-text align-self-center px-2">
          <small class="text-muted ">{{link.name}} </small> <br>
          <small class="text-muted ">{{link.position}}</small>
      </p>
      </div>
    </div>
    </div>
    <div class="text-center pt-5">
      <i class="fas fa-circle"></i><i class="fas fa-circle"></i><i class="fas fa-circle"></i>
    </div>
  </div>
</template>

<script>
export default {
  name: "FeedBack",
  data() {
    return {
      feedBackList: [
        {
          img: require("@/assets/images/testimonial/artist-testimonial-avatar-04.jpg"),
          alt: "feedback",
          title: "High level of efficiency and scientific teaching methods",
          text: "I am free to learn at my own pace, follow my own schedule and choose the subject I want to learn from the syllabus. Great study portal for people like me.",
          name:"Mina Hollace",
          position:"/ Freelance",
        },
        {
          img: require("@/assets/images/testimonial/artist-testimonial-avatar-01.jpg"),
          alt: "feedback",
          title: "Professional team of specialists and passionate mentors at reach ",
          text: "I need to get a certification for English proficiency and MaxCoach is my best choice. Their tutors are smart and professional when dealing with students.",
          name:"Madley Pondor",
          position:"/ IT Specialist",
        },
        {
          img: require("@/assets/images/testimonial/artist-testimonial-avatar-02.jpg"),
          alt: "feedback",
          title: "The MaxCoach team works really hard to ensure high quality",
          text: "I am happy with their arrangement of lessons and subjects. They reflect a scientific  investigation into effective methods to be adopted for learners of all levels.",
          name:"Luvic Dubble",
          position:"/ Private Tutor",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style/_commons.scss";
@import "../assets/style/_variables.scss";

h2 {
  color: $Cerulean;
  font-family: "Satisfy", cursive;
}
h4 {
  font-weight: bold;
}
.ms_opacity{cursor: pointer;}
.ms_opacity:nth-child(odd){
    opacity: 0.5;
    
      &:hover{
        opacity: 1;
        
      }

  } 
  .fa-circle{
    font-size: 7px;
    margin-left: 2%;
    color: $Silver;
      &:first-child{
        color: black;
        font-size: x-small;
      }
  }

img{
    width: 75px;
}
</style>
