<template>
  <!-- Main (9 sezioni) -->
  <main>
    <!-- Modalità corsi -->
    <section class="container-fuid">
       <CoachComp /> 
    </section>

    <!-- Text -->
       <section id="about" class="container-fluid">
           <div class="wrapper ">
               <div class="container">
                    <div class="row">
                        <div class="col-xs-12 col-sm-6 text-center">
                            <img src="@/assets/images/artist-quote-icon.png" alt="">
                            <p class="">
                                I coach and mentor visual artists, like you, to Create Like You Mean It	
                                
                            </p>
                            <p>Martin Garrix</p>
                        </div>
                        <div class="col-xs-12 col-sm-6">
                            <p class="text-left">
                                As a coach and mentor, my ultimate goal is to motivate visual artists toward inspired action. I help you get you back on track to being the productive, creative, meaningful and authentic artist you truly want to be.I support artists in crafting and living a creative life as well as feeling good about themselves and their art.
                            </p>  
                            <p>
                                As an artist and an educator for nearly 30 years, I understand what it takes to create.
                            </p>                         
                            <a class="btn btn-default" href="#" role="button">
                                <span>Get Started</span>
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    <!-- Fake video -->
    <section class="" id="ms_video">
        <VideoComp/>

    </section>

    <!-- Testimonianze -->
    <section></section>

    <!-- Corsi Online -->
    <section></section>

    <!-- Ultime dal Blog -->
    <section></section>

    <!-- Eventi -->
    <section></section>

    <!-- Newsletter -->
    <section id="newsletter" class="d-flex justify-content-center align-middle">
      <div class="wrapper">
        <div class="container-fluid">
          <div class="row">
            <div class="col-xs-12 col-sm-6">
              <p class="text-left">Newsletter</p>
            </div>
            <div class="col-xs-12 col-sm-6">
              <input type="email" placeholder="email" />
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Fine Main -->
  </main>
</template>

<script>
import CoachComp from "./CoachComp.vue";
import VideoComp from "./VideoComp.vue"

export default {
  name: 'MainComp',
  components: {
    CoachComp,
    VideoComp
}
}
</script>

<style lang="scss" scoped>
@import "../assets/style/_commons.scss";
@import "../assets/style/_variables.scss";

#newsletter {
  background-color: $BayofMany;
  height: 20vh;
  background-image: url("@/assets/images/Sagome/artist-shape-color-paint-bottom-right-300x153.png"),
    url("@/assets/images/Sagome/artist-shape-color-paint-top-left-300x170.png");
  background-position: right bottom, left bottom;
  background-repeat: no-repeat;
  background-size: contain;
}
</style>
