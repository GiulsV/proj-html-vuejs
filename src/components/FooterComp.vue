<template>
  <!-- Footer dinamico-->
  <footer>
    <div
      class="container d-flex justify-content-between text-dark ms_padding"
      id="ms_container"
    >
      <!-- sezione indirizzo -->
      <section id="address" class="d-flex flex-wrap">
        <h5>Address</h5>
        <p>
          382 NE 191st St # 87394 Miami, FL 33179-3899 <br />
          +1 (305) 547-9909 (9am - 5pm EST, Monday - Friday) <br />
          support@maxcoach.com
        </p>

        <div class="d-flex">
          <ul class="list-group list-group-horizontal">
            <li class="list-group-item border-0">
              <a class="ms_social_icon" href="#">
                <i class="fab fa-twitter border-0"></i>
              </a>
            </li>
            <li class="list-group-item border-0">
              <a class="ms_social_icon" href="#">
                <i class="fab fa-facebook-f"></i>
              </a>
            </li>
            <li class="list-group-item border-0">
              <a class="ms_social_icon" href="#">
                <i class="fab fa-instagram"></i>
              </a>
            </li>
            <li class="list-group-item border-0">
              <a class="ms_social_icon" href="#">
                <i class="fab fa-linkedin"></i>
              </a>
            </li>
          </ul>
        </div>
      </section>

      <!-- sezione explore -->
      <div class="ms_list">
        <h5>Explore</h5>
        <ul class="list-group">
          <li
            class="list-group-item border-0"
            v-for="(link, index) in exploreLink"
            :key="index"
          >
            <a :href="link.src" class="">
              {{ link.label }}
            </a>
          </li>
        </ul>
      </div>
      <!-- sezione info -->
      <div class="ms_list">
        <h5>Information</h5>
        <ul class="list-group">
          <li
            class="list-group-item border-0"
            v-for="(link, i) in infoLink"
            :key="i"
          >
            <a :href="link.src" class="">
              {{ link.label }}
            </a>
          </li>
        </ul>
      </div>

      <!-- sezione Instagram -->

      <div class="d-flex flex-column">
        <h5>Instagram <a href="#" id="link_insta">@maxcoach</a></h5>
        <ul class="list-group list-group-horizontal">
          <li
            class="list-group-item border-0 p-2"
            v-for="(link, y) in imageLink"
            :key="y"
          >
            <img :src="link.img" :alt="link.alt" class="insta_img" />
          </li>
        </ul>
      </div>
    </div>
    <div class="ms_toppage text-center">
      <p><i class="far fa-copyright"></i>2020 Maxcoach. All Rights Reserved</p>
      <a href="#top" class="rounded-circle"><i class="fas fa-arrow-up"></i></a>
    </div>

    <!-- copyrigth -->
  </footer>
  <!-- fine footer -->
</template>

<script>
export default {
  name: "NavBar",
  data() {
    return {
      exploreLink: [
        {
          label: "Start here",
          src: "#",
        },
        {
          label: "Success story",
          src: "#",
        },
        {
          label: "Blog",
          src: "#",
        },
        {
          label: "Courses",
          src: "#",
        },
        {
          label: "Contact us",
          src: "#",
        },
      ],
      infoLink: [
        {
          label: "Membership",
          src: "#",
        },
        {
          label: "Purchase guide",
          src: "#",
        },
        {
          label: "Privacy policy",
          src: "#",
        },
        {
          label: "Terms of services",
          src: "#",
        },
      ],
      imageLink: [
        {
          img: require("@/assets/images/Insta/120084500_197897808368764_8114555493043279565_n.jpg"),
          alt: "Insta img",
        },
        {
          img: require("@/assets/images/Insta/120012142_177596140500760_8623485824101406058_n.jpg"),
          alt: "Insta img",
        },
        {
          img: require("@/assets/images/Insta/120099363_364334431619755_7198812647386067017_n.jpg"),
          alt: "Insta img",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style/_commons.scss";
@import "../assets/style/_variables.scss";
#ms_container {
  flex-basis: calc(100% / 4);
  font-size: small;
  color: #797979;
}
#address {
  width: 25%;
  // color: black;
}
.insta_img {
  width: 150px;
}
.ms_social_icon {
  color: #bcbcbc;
  font-size: 25px;
}
#link_insta {
  color: #a65d50;
}

.ms_toppage {
  a {
    position: relative;
    float: right;

    margin-bottom: 2rem;
    margin-right: 2rem;
    width: 45px;
    height: 45px;
    background-color: $Orangebtn;
    i {
      font-size: 20px;
      color: white;
      padding: 10px;
    }
    p {      
      color:#bcbcbc;
      font-size: 6px;
    }
  }
}
</style>
