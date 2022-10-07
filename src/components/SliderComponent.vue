<template>
  <div class="container">
    <div class="slides">
        <p>REAL STORIES</p>
        <div class="slide" v-for="slide in slides" :key="slide.id">
            <div class="active" v-if="slide.id === order">
                <p>{{slide.description}}</p>
                <img :src="require(`@/assets/motivation/images/${slide.thumb}`)" alt="">
            </div>
        </div>
        <div class="round-button">
            <div class="prev" @click="prevImage">&and;</div>
            <div class="next" @click="nextImage">&or;</div>
            
        </div>
    </div>

    <div class="fixed">
        <img src="../assets/motivation/images/home-movation-testimonial-image.jpg" alt="">
    </div>
  </div>
</template>

<script>
export default {
    name:'SliderComponent',
    props:{
        slides:Array,

    },
    data(){
        return {
            order:1,
        }
    },
    methods:{
        nextImage(){
            if(this.order===this.slides.length){
                this.order=1;
            }
            else
                this.order++;
        },

        prevImage(){
            if(this.order===1)
                this.order=this.slides.length;
            else
                this.order--;
        }
    }

}


</script>

<style scoped lang="scss">
    .container{
        width: 100%;
        display: flex;
        .slides{
             width: 50%;
            .round-button{
                background: red;
                width: 100px;
                height: 100px;
                -moz-border-radius: 50px;
                -webkit-border-radius: 50px;
                border-radius: 50px;
                background-color: red;
                display: flex;
                flex-direction: column;
                justify-content: center;
            }
            .slide{
                .active{
                    img{
                        width: 100%;
                    }
                }
            }
           
        }
        .fixed{
            width: 50%;
            img{
                width: 100%;
            }
        }
    }
    
</style>