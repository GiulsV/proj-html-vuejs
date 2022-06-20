<template>
  <div class="container">
    <div class="card mb-3" style="max-width: 540px" v-for="(event, i) in eventCards" :key="i">
      <div class="row g-0">
        <div class="col-md-4" >
          <img
            class="img-fluid rounded-start" :src="event.img" :alt="event.alt"
          />
        </div>
        <div class="col-md-8">
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
</template>

<script>
export default {
  name: "EventComp",
  data() {
    return {
      eventCards: [
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
        {
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

<style lang="scss" scoped></style>
