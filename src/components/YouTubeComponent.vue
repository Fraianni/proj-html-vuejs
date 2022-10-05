<template>
    <div class="container">
        <div class="video">
            <div class="video_preview">
                <img class="person" src="../assets/motivation/images/home-movation-video-poster-670x450.jpg" alt="">
                <img class="play" src="../assets/motivation/images/icon-youtube-play.png" alt="">

            </div>
            <div class="video_info">
                <p>"Every morning you have two choices: continue to sleep with your dreams, or wake up and chase them."</p>
                <img src="../assets/motivation/images/home-movation-shape-01.png" alt="">
                <h3>Kaixa Stark</h3>
                <span>WINGMAN</span>
            </div>
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
        display: flex;
        justify-content: center;
    }
    .video{
        margin-top: 100px;
        display: flex;
        justify-content: space-between;
        width: 1400px;
        .video_preview{
            position: relative;
            flex-grow:0.5;
            .person{
                width: 100%;
            }
            .play{
                position:absolute;
                left: 50%;
                top: 45%;
                transform: translateX(-50%);
                &:hover{
                    filter: grayscale(50%);
                  
                }
                

            
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