<template>
  <div class="container">
    <div class="video_preview">
        <img src="../assets/motivation/images/home-movation-video-poster-670x450.jpg" alt="">
    </div>
    <div class="video_info">
        <p>"Every morning you have two choices: continue to sleep with your dreams, or wake up and chase them."</p>
        <img src="../assets/motivation/images/home-movation-shape-01.png" alt="">
        <h3>Kaixa Stark</h3>
        <span>WINGMAN</span>
    </div>
  </div>
</template>

<script>
export default {
    name:'YouTubeComponent'
}
</script>

<style scoped lang="scss">
    .container{
        margin-top: 100px;
        display: flex;
        justify-content: space-around;
        .video_preview{
            img{
                width: 100%;
            }
        }
        .video_info{
            max-width: 500px;
            text-align: left;
            display: flex;
            flex-direction: column;
            justify-content: center;
            p{
                font-size: 2rem;
            }
            img{
                width: 30px;
                margin-top: 50px;
            }
            h3{
                margin:30px 0px
            }
            span{
                color:grey
            }
        }
    }
</style>