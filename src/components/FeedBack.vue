<template>
  <div class="container">
    <h2>Testimonials</h2>
    <h4>Why do people love me?</h4>
    <div class="card" v-for="(link, i) in feedBackList" :key="i">
      <div class="card-body">
        <h5 class="card-title">{{link.title}}</h5>
        <p class="card-text">
            {{link.text}}
        </p>

      </div>
      <img :src="link.img" :alt="link.alt" class="card-img-bottom"/>
      <p class="card-text">
          <small class="text-muted">{{link.name}} {{link.position}}</small>
        </p>
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
          position:"/Freelance",
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

img{
    width: 50px;
    border-radius: 50%;
}
</style>
