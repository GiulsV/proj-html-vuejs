<template>
<!-- Header -->
<header>
    <!-- Section countdown -->
    <section class="container-fluid d-flex flex-row justify-content-center" id="countdown">
        <p class="align-self-center"> Start tomorrow our biggest event of the year <i class="far fa-clock"></i> 00:00:00:00 <button>GET ticket</button></p>
        
    </section>

    <!-- Header Navigazione Dinamico-->
    <NavBar />

</header>
<!-- Fine Header -->
</template>

<script>
import NavBar from "@/components/NavBar.vue"

export default{
    name: 'HeaderComp',
    components:{
        NavBar
    }
}
</script>

<style lang="scss" scoped>
#countdown{
    background-color: #F4F0EF;
}

</style>