<template>
  <!-- Main (9 sezioni) -->
  <main>
    <!-- Modalità corsi -->
    <section class="ms_default"></section>

    <!-- Text -->
    <section></section>

    <!-- Fake video -->
    <section></section>

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
                            <p class="text-left">
                                News letter
                            </p>
                        </div>
                        <div class="col-xs-12 col-sm-6">
                            <input type="email" placeholder="email">
                        </div>
                    </div>
                </div>
            </div>
        </section>

    <!-- Fine Main --> 
  </main>

</template>

<script></script>

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
