<template>
  <!-- Main (8 sezioni) -->
  <main>
    <!-- Modalità corsi -->
    <section class="ms_padding ms_coach">

       <CoachComp /> 
    </section>

    <!-- Text -->
       <section id="about" class="container-fluid ms_padding">
           <div class="wrapper ">
               <div class="container">
                    <div class="row">
                        <div class="col-xs-12 col-sm-6 text-center ms_text_bold">
                            <img src="@/assets/images/artist-quote-icon.png" alt="">
                            <p class="">
                                I coach and mentor visual artists, like you, to Create Like You Mean It	
                                
                            </p>
                            <p>Martin Garrix</p>
                        </div>
                        <div class="col-xs-12 col-sm-6 align-items-center ms_text_normal">
                            <p class="text-left">
                                As a coach and mentor, my ultimate goal is to motivate visual artists toward inspired action. I help you get you back on track to being the productive, creative, meaningful and authentic artist you truly want to be.I support artists in crafting and living a creative life as well as feeling good about themselves and their art.
                            </p>  
                            <p>
                                As an artist and an educator for nearly 30 years, I understand what it takes to create.
                            </p>                         
                            <a class="btn bt_red" href="#" role="button">Get Started</a> 
                        </div>
                    </div>
                </div>
            </div>
        </section>
    <!-- Fake video -->
    <section class="ms_padding" id="ms_video">
        <VideoComp/>

    </section>

    <!-- Testimonianze -->
    <section class="wrapper ms_padding  ms_feedback">
      <FeedBack/>
    </section>

    <!-- Corsi Online -->
    <section class="ms_padding bg_course">
        <CourseComp/>
    </section>

    <!-- Blog -->
    <section class="wrapper ms_padding">
      <BlogComp/>
    </section>

    <!-- Eventi -->
    <section class="ms_padding bg_image">
      <EventComp/>
    </section>

    <!-- Newsletter -->
    <section id="newsletter" class="d-flex justify-content-center align-items-center ms_padding">
      <div class="container">  
          <div class="row ">
            <div class="col-5 ms_text_news">
              <p class="text-end ">Newsletter to get in touch</p>
            </div>
            <div class="form__group field">
              <input type="input" class="form__field" placeholder="Name" name="name" id='name' required />
              <label for="name" class="form__label">Your email<i class="fa-solid fa-arrow-right ms_arrow"></i></label>
            </div>
          </div>
        </div>
    </section>

    <!-- Fine Main -->
  </main>
</template>

<script>
import CoachComp from "./CoachComp.vue";
import VideoComp from "./VideoComp.vue";
import CourseComp from "./CourseComp.vue";
import BlogComp from "./BlogComp.vue"
import EventComp from "./EventComp.vue"
import FeedBack from "./FeedBack.vue"

export default {
  name: 'MainComp',
  components: {
    CoachComp,
    VideoComp,
    CourseComp,
    BlogComp,
    EventComp,
    FeedBack
}
}
</script>

<style lang="scss" scoped>
@import "../assets/style/_commons.scss";
@import "../assets/style/_variables.scss";

.ms_coach{
  background-image: url('@/assets/images/Sagome/maxcoach-shape-14.png');
  background-repeat: no-repeat;
  background-size: contain;
  background-position: top 20% right ;
  

}

#about{
  height: 60%;
  
  .ms_text_bold{
    padding: 0 7rem;
    font-size: 40px;
    font-weight: bold;
  }
  .ms_text_normal{
    text-align: left;
    padding: 4rem 5rem;
    color: $Boulder;
    p{
      padding:1rem 0;
    }


  }

}

.bg_course{
  background-image: url('@/assets/images/Sagome/artist-shape-01-600x577.png');
  background-repeat: no-repeat;
  background-position: top 5% right;
}
.bg_image{
  background-image: url('@/assets/images/Sagome/maxcoach-shape-13.png');
  background-repeat: no-repeat;
  background-position: top 5% right;
}
.ms_feedback{
  background-color: #FAF8F6;
}

#newsletter {
  background-color: $BayofMany;
  height: 20vh;
  background-image: url("@/assets/images/Sagome/artist-shape-color-paint-bottom-right-300x153.png"),
    url("@/assets/images/Sagome/artist-shape-color-paint-top-left-300x170.png");
  background-position: right bottom, left bottom;
  background-repeat: no-repeat;
  background-size: contain;
    .ms_text_news{
      padding:0 8rem;
      color: white;
      p{
      font-size: 35px;
      }  
    }
    .form__group {
  position: relative;
  padding: 15px 0 0;
  margin-top: 10px;
  width: 50%;
}

.form__field {
  font-family: inherit;
  width: 80%;
  border: 0;
  border-bottom: 1px solid $DustGray;
  outline: 0;
  font-size: 1.3rem;
  color: white;
  padding: 7px 0;
  background: transparent;
  transition: border-color 0.2s;

  &::placeholder {
    color: transparent;
  }

  &:placeholder-shown ~ .form__label {
    font-size: 1.3rem;
    cursor: text;
    top: 20px;
  }
}

.form__label {
  position: absolute;
  top: 0;
  display: block;
  transition: 0.2s;
  font-size: 1rem;
  color: white;
}

.form__field:focus {
  ~ .form__label {
    position: absolute;
    top: 0;
    display: block;
    transition: 0.2s;
    font-size: 1rem;
    color: white;
    font-weight:700;    
  }
  padding-bottom: 6px;  
  font-weight: 700;
  border-width: 2px;
  border-image-slice: 1;
}
.ms_arrow{
  padding-left: 25rem;
}
}
</style>
