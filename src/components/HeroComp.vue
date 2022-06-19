<template>
<div class="jumbotron jumbotron-fluid d-flex " id="hero">
    <!-- justify-content-between -->
    <!-- <img src="@/assets/images/Sagome/artist-shape-02.png" alt=""/>
    <img src="@/assets/images/Sagome/artist-shape-01.png" alt=""/> -->
    <div class="container d-flex flex-column justify-content-center text-center" id="text_jumbo">
        <div class="wrapper">
            <h1>Hello I'm Martin</h1>
            <h3>Artist Coaching And Mentoring </h3>
            <h3> Might Be for You.</h3>
            <a class="btn bt_orange" href="#" role="button">Get Started Today</a> 
        </div>

    </div>



</div>

</template>

<script>
</script>

<style lang="scss" scoped>
@import "../assets/style/_commons.scss";
@import "../assets/style/_variables.scss";

#hero{
    // background-color: #FBF9F6;
    // background-color: blue;
    height: 80vh;
    background-image: url('@/assets/images/Sagome/artist-shape-02.png'), url('@/assets/images/Sagome/artist-shape-01.png'),  url('@/assets/images/Sagome/artist-shape-03-201x300.png'), url('@/assets/images/Sagome/artist-shape-04-127x300.png');

    background-repeat: no-repeat;
    background-size:fill;
    background-position: 
            top left, 
            top right 6%,
            bottom 2% left 8%,
            right 15% top 10%;
}
// button{
//     width: 100px;
// }
</style>