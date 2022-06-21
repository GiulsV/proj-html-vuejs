<template>
  <div class="container-fluid ">
    <div class="text-center ms_padding_title">
    <h2>Upcoming Event</h2>
    <h4>Let's work togheter</h4>
    </div>
    
    <div class="container">
   <div class="row justify-content-around ">
    <div class="card mb-3 rounded-0 border-0"  v-for="(event, i) in eventCardsFirst" :key="'A'+ i">
      <div class="row g-0" >
        <div class="col-4 " >
          <img
            class="img-fluid rounded-0" :src="event.img" :alt="event.alt"
          />
        </div>
        <div class="col-8">
          <div class="card-body"> 
            <p class="card-text" >
               {{ event.date }}
            </p>
            <h5 class="card-title">{{ event.title }}</h5>
            <p class="card-text" >
               {{ event.text }}
            </p>
            <p class="card-text">
              <small class="text-muted"><i class="fas fa-map-marker-alt"></i>{{event.place}}</small>
            </p>
          </div>
        </div>
      </div>
       </div>
       </div>

  <div class="row justify-content-around ms_event ms_padding_title">
    <div class="card mb-3 rounded-0 border-0"  v-for="(event, i) in eventCardsSecond" :key="'B'+i">
      <div class="row g-0" >


        <div class="col-8">
          <div class="card-body"> 
            <p class="card-text" >
               {{ event.date }}
            </p>
            <h5 class="card-title">{{ event.title }}</h5>
            <p class="card-text" >
               {{ event.text }}
            </p>
            <p class="card-text">
              <small class="text-muted"><i class="fas fa-map-marker-alt"></i>{{event.place}}</small>
            </p>
          </div>
        </div>
        <div class="col-4 " >
                  <img
            class="img-fluid rounded-0" :src="event.img" :alt="event.alt"
          />
        </div>
      </div>
       </div>
       </div>
    </div>
    </div>

    </template>

<script>
export default {
  name: "EventComp",
  data() {
    return {
      eventCardsFirst: [
        {
          img: require("@/assets/images/event/artist-event-01-250x300.jpg"),
          alt: "event",
          date:"Nov 22, 2020",
          title: "The Acrylic Painting Academy",
          text: "Texas,USA",
        },
        {
          img: require("@/assets/images/event/artist-event-02-250x300.jpg"),
          alt: "event",
          date:"Nov 22, 2020",
          title: "Drawing and Shading:Complete Course",
          text: "Texas,USA",
        },
        ],
        
        eventCardsSecond:[{
          img: require("@/assets/images/event/artist-event-03-250x300.jpg"),
          alt: "event",
          date:"Nov 22, 2020",
          title: "The Color Theory for Digital Artist",
          text: "Texas,USA",
        },
        {
          img: require("@/assets/images/event/artist-event-04-250x300.jpg"),
          alt: "event",
          date:"Nov 22, 2020",
          title: "Ultimate Guide To Digital Sketching for Beginner",
          text: "Texas,USA",
        },
      ],
    };
  },
};

</script>

<style lang="scss" scoped>
@import "../assets/style/_commons.scss";
@import "../assets/style/_variables.scss";

h2{
  color:$Cerulean;
  font-family: 'Satisfy', cursive;
}
h4{
  font-weight: bold;
}
.card{
  max-width: 540px;
}
.ms_event{
      margin-left: 100px;
}

</style>
