<template>
  <!-- Header -->
  <header>
    <!-- Section countdown -->
    <section
      class="container-fluid d-flex flex-row justify-content-center"
      id="countdown"
    >
      <p class="align-self-center">
        Start tomorrow our biggest event of the year
        <i class="far fa-clock"></i> 00:00:00:00
        <a class="btn bt_orange" href="#" role="button">Get Ticket</a>
      </p>
    </section>
    <!-- Header Navigazione Dinamico-->
    <section>
      <NavBar />
    </section>

    <!-- Jumbotron -->
    <section id="ms_hero">
      <HeroComp />
    </section>
  </header>
  <!-- Fine Header -->
</template>

<script>
import NavBar from "@/components/NavBar.vue";
import HeroComp from "@/components/HeroComp.vue";

export default {
  name: "HeaderComp",
  components: {
    NavBar,
    HeroComp,
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style/_commons.scss";
@import "../assets/style/_variables.scss";
#countdown {
  background-color: #f4f0ef;
}
#ms_hero {
  background-color: #fbf9f6;
  height: 80vh;
  background-image: url("@/assets/images/Sagome/artist-shape-02.png"),
    url("@/assets/images/Sagome/artist-shape-01.png");
  background-position: top left, top right 6%;
  background-repeat: no-repeat;
//   background-size: contain;
}
</style>
