<template>
  <div class="container-fluid bg_hero_image" id="bg_hero">
    <div class="container h-100 d-flex justify-content-around">
      <div class="row flex-nowrap align-items-center">
        <div class="col">
          <img src="@/assets/images/Jumbo/artist-hero-image-02.jpg" alt="img" />
        </div>
        <div class="col-4 flex-grow-1 justify-content-center text-center">
          <h1 class="lh-lg">Hello I'm Matin</h1>
          <h3 class="lh-lg">Artist Coaching And Mentoring</h3>
          <h3 class="lh-lg">Might Be for You.</h3>
          <a class="btn bt_orange" href="#" role="button">Get Started Today</a>
        </div>
        <div class="col">
          <img src="@/assets/images/Jumbo/artist-hero-image-04.jpg" alt="img" />
        </div>
      </div>

      <div class="ms_jumbo">
        <img src="@/assets/images/Jumbo/artist-hero-image-01.jpg" alt="" />
        <!-- <img src="@/assets/images/Jumbo/artist-hero-image-03.png" alt=""> -->
      </div>
    </div>
  </div>
</template>

<script></script>

<style lang="scss" scoped>
@import "../assets/style/_commons.scss";
@import "../assets/style/_variables.scss";

#bg_hero {
  background-image: url("@/assets/images/Sagome/artist-shape-05.png"),
    url("@/assets/images/Sagome/maxcoach-shape-12.png"),
    url("@/assets/images/Sagome/artist-shape-03.png");
  background-repeat: no-repeat;
  background-position: bottom right 2%, bottom 3% right 10%, bottom 50% left 5%;
  background-size:auto, auto, 15rem;
}

h1 {
  color: $Cerulean;
  font-family: "Satisfy", cursive;
}

.row > .col:last-of-type {
  padding-top: 4rem;
  margin-left: 5rem;
}

.row > .col:first-of-type {
  padding-bottom: 8rem;
  margin-right: 5rem;
  margin-left: 5rem;
}

.ms_jumbo {
  position: absolute;
  top: 50%;
  left: 5%;
}

img {
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
}
</style>
