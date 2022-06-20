<template>
<div class="container">
    <div id="ms_video" class="d-flex justify-content-center position-relative">
        <img src="@/assets/images/video/artist-video-poster.jpg" alt="video">    
        <div id="yt_play" class="position-absolute top-50 start-50 translate-middle">
            <img src="@/assets/images/video/icon-youtube-play.png" alt="yt">
        </div>
    </div>

</div>
</template>

<script>

</script>

<style lang="scss" scoped>
#ms_video{
    padding: 60px 0;
    background-image: url('@/assets/images/Sagome/maxcoach-shape-05-150x150.png'), 
                      url('@/assets/images/Sagome/maxcoach-shape-12-150x150.png');
    background-position: top 5% left 10%,
                        bottom 5% right 5%;
    background-repeat: no-repeat;
}


</style>