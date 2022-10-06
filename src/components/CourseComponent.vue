<template>
  <div class="card">
    <img :src="require(`@/assets/motivation/images/${course.thumb}`)" alt="">
    <div class="text">
        <h2>{{course.price}}</h2>
        <p>{{course.description}}</p>
    </div>
    
  </div>
</template>

<script>
export default {
    name:'CourseComponent',
    props:{
        course:Object,

    }
}
</script>

<style scoped lang="scss">
    .card{
        display: flex;
        flex-direction: column;
        text-align:left;
        margin: 10px;
        .text{
            margin-left: 30px;
            img{
                width: 100%;
            }
            h2{
                color:#20ac97;
                margin-bottom: 10px;
            }
        }
      
    }
</style>