<template>
  <main>
    <PanoramaComponent />
    <!-- <img :src="require(`@/assets/motivation/images/${courses[0].thumb}`)" alt=""> -->
    <!-- <img :src="require(`@/assets/motivation/images/${this.courses[0].thumb}`)" alt=""> -->
    <div class="courses-titles">
      <h3>Begin your journey at MaxCoach</h3>
      <h1>Latest <span>Online Courses</span> </h1>
    </div>
    <CoursesComponent :courses="courses" />
     
  </main>
</template>

<script>
import courses from '../assets/data/courses.json'
import PanoramaComponent from './PanoramaComponent.vue'
import CoursesComponent from './CoursesComponent.vue'
export default {
    name:'MainComponent',

    components:{
        PanoramaComponent,
        CoursesComponent
        
    },
    // props:{
    //   courses:Array,

    // },
    data(){
    return {
      courses
    }
  }
}
</script>

<style scoped lang="scss">
  .courses-titles{
    margin: 50px 0px;
    h3{
      color: gray;
    }
    span{
      color:#20ac97;
    }
  }

</style>