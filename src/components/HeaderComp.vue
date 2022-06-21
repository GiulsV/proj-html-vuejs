<template>
  <!-- Header -->
  <header>
    <!-- Section countdown -->
    <section
      class="container-fluid d-flex flex-row justify-content-center"
      id="countdown"
    >
      <small class="align-self-center text-muted px-2">
        Start tomorrow our biggest event of the year...
        <i class="far fa-clock px-2"> 00 : 00 : 00 : 00</i>
        <a class="btn bt_orange px-2" href="#" role="button">Get Ticket</a>
      </small>
    </section>
    <!-- Header Navigazione Dinamico-->
    <section>
      <NavBar />
    </section>

    <!-- Jumbotron -->
    <section id="ms_hero" class="jumbotron-fluid d-flex">
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
  height: 40px;
  i {
    color: $CodGray;
  }
}
#ms_hero {
  background-color: #fbf9f6;
  background-image: url("@/assets/images/Sagome/artist-shape-02.png"),
    url("@/assets/images/Sagome/artist-shape-01.png");
  background-position: top left, top right 6%;
  background-repeat: no-repeat;
  //   background-size: contain;

  height: 70vh;
  vertical-align: middle;
}
</style>
