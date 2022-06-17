<template>
    <nav class="navbar navbar-expand-lg navbar-light bg-white text-dark">
        <!-- Logo a sinistra-->
        <a class="navbar-brand">
            <img src="../assets/images/logo/dark-logo.png" alt="Logo">
        </a>
        <!-- Navbar in centro-->
        <div>
            <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                <li class="nav-item mx-0 mx-lg-1"
                    v-for="(link, index) in navLink"
                    :key="index">
                    <a :href="link.src" class="nav-link py-3 px-0 px-lg-3 text-dark">
                        {{link.label}}<i class="fas fa-chevron-down"></i>
                    </a>
                </li>
            </ul>
            <!-- Icone social a destra -->
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
</template>


<script>
export default {
    name: "NavBar",
    data() {
        return {
            navLink: [
                {
                    label: "Home",
                    src: "#"
                },
                {
                    label: "Pages",
                    src: "#"
                },
                {
                    label: "Courses",
                    src: "#"
                },
                {
                    label: "Features",
                    src: "#"
                },
                {
                    label: "Blog",
                    src: "#"
                },
                {
                    label: "Shop",
                    src: "#"
                },
            ]
            
        }
    }
}
</script>

<style lang="scss" scoped>


</style>