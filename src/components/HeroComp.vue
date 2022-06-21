<template>

    <div class="container d-flex justify-content-around">
      <div class="row flex-nowrap align-items-center">
        <div class="col border">
         
         <img src="@/assets/images/Jumbo/artist-hero-image-02.jpg" alt="img" />
          
        </div>
        <div
          class="col-4 flex-grow-1 border justify-content-center text-center "
          id="text_jumbo"
        >
          <h1 class="lh-lg">Hello I'm Matin</h1>
          <h3 class="lh-lg">Artist Coaching And Mentoring</h3>
          <h3 class="lh-lg">Might Be for You.</h3>
          <a class="btn bt_orange" href="#" role="button">Get Started Today</a>
        </div>
        <div class="col border">
          <img src="@/assets/images/Jumbo/artist-hero-image-04.jpg" alt="img" />
        </div>
      </div>
    </div>

</template>

<script></script>

<style lang="scss" scoped>
@import "../assets/style/_commons.scss";
@import "../assets/style/_variables.scss";
h1 {
  color: $Cerulean;
  font-family: "Satisfy", cursive;
}

 .row > .col:last-of-type{
     padding-top: 8rem;
     margin-left: 6rem;
 }

 .row > .col:first-of-type{
     padding-bottom: 8rem;
     margin-right: 10rem;
 }

//  #text_jumbo{
//      width: 200px;
//  }
</style>
