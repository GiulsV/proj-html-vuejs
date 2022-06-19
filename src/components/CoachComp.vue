<template>
  <div class="wrapper ">
    <div class="container ms_coach_card">
      <div class="text-center">
        <h2>Artist coaching</h2>
        <h4>I understand what it takes to create.</h4>
        <h4>I can help you with</h4>
      </div>
      <div class="row d-flex justify-content-center " >
      <div class="col" v-for="(link, index) in coachCard" :key="index" id="ms_corsi">
        <div class="card border-0">
          <img class="card-img-top rounded-0" :src="link.img" :alt="link.alt" />
          <div class="card-body ms_card_body">
            <p class="card-title mt-3">{{ link.title }}</p>

            <p class="card-text">
              <small class="text-muted">{{ link.text }}</small>
            </p>
          </div>
        </div>
      </div>
    </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CourseComp",
  data() {
    return {
      coachCard: [
        {
          img: require("@/assets/images/box/artist-box-image-01.png"),
          alt: "corso",
          title: "Online Coures",
          text: "Online art coaching now offers you a very powerful way to redesign your artist mind.",
        },
        {
          img: require("@/assets/images/box/artist-box-image-02.png"),
          alt: "corso",
          title: "One to One",
          text: "Getting the necessary clarity about the current state to help you improve your ability.",
        },
        {
          img: require("@/assets/images/box/artist-box-image-03.png"),
          alt: "corso",
          title: "Anywhere",
          text: "Access to valuable and portable program which allow you to setup and live anywhere you want.",
        },
        {
          img: require("@/assets/images/box/artist-box-image-04.png"),
          alt: "corso",
          title: "On Time",
          text: "Punctuality is our top priority because it's an essential criteria to assess a program quality.",
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
  width: 50%;
}
</style>
