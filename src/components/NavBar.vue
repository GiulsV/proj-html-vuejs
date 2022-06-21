<template>
  <div class="container d-flex flex-column flex-nowrap">
    <!-- <div class="row"> -->
      <!-- <div class="col-xs-12"> -->
        <nav class="navbar navbar-expand-lg navbar-light bg-white text-dark justify-content-between">
        <!-- Logo a sinistra-->
        <div class="logo d-flex flex-row justify-content-center">
          <a class="navbar-brand">
            <img src="../assets/images/logo/dark-logo.png" alt="Logo" />
          </a>
        </div>

        <!-- Navbar in centro-->
        
          <div class="d-flex flex-row justify-content-center">
            <ul class="navbar-nav me-auto mb-2 mb-lg-0">
              <li
                class="nav-item mx-0 mx-lg-1"
                v-for="(link, index) in navLink"
                :key="index"
              >
                <a
                  :href="link.src"
                  class="nav-link py-3 px-0 px-lg-3 text-dark"
                >
                  {{ link.label }} <small><i class="fas fa-chevron-down text-muted"></i></small>
                </a>
              </li>
            </ul>
          </div>
        
        <!-- Icone social a destra -->
        <div class="d-flex flex-row justify-content-center">
          <ul class="navbar-nav mb-2 mb-lg-0">
            <li class="nav-item mx-0 mx-lg-1">
              <a class="nav-link py-3 px-0 px-lg-3 text-dark" href="#">
                <i class="fab fa-twitter"></i>
              </a>
            </li>
            <li class="nav-item mx-0 mx-lg-1">
              <a class="nav-link py-3 px-0 px-lg-3 text-dark" href="#">
                <i class="fab fa-facebook-f"></i>
              </a>
            </li>
            <li class="nav-item mx-0 mx-lg-1">
              <a class="nav-link py-3 px-0 px-lg-3 text-dark" href="#">
                <i class="fab fa-instagram"></i>
              </a>
            </li>
            <li class="nav-item mx-0 mx-lg-1">
              <a class="nav-link py-3 px-0 px-lg-3 text-dark" href="#">
                <i class="fab fa-linkedin"></i>
              </a>
            </li>
          </ul>
        </div>
        </nav>
      <!-- </div> -->
    <!-- </div> -->
  </div>
</template>

<script>
export default {
  name: "NavBar",
  data() {
    return {
      navLink: [
        {
          label: "Home",
          src: "#",
        },
        {
          label: "Pages",
          src: "#",
        },
        {
          label: "Courses",
          src: "#",
        },
        {
          label: "Features",
          src: "#",
        },
        {
          label: "Blog",
          src: "#",
        },
        {
          label: "Shop",
          src: "#",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style/_commons.scss";
@import "../assets/style/_variables.scss";
.logo img {
  width: 8rem;
}
.fa-chevron-down{
 font-size: 9px;
 vertical-align: middle;
}
i > .fab{
  color: $Boulder;
}
</style>
