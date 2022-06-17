<template>
<!-- Header -->
<header>
    <!-- Section countdown -->

    <!-- Header Navigazione Dinamico-->
    <div class="container">
        <NavBar />      

    </div>

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

</style>