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
    <button>View all courses</button>
    <BooksComponent />
     
  </main>
</template>

<script>
import courses from '../assets/data/courses.json'
import PanoramaComponent from './PanoramaComponent.vue'
import CoursesComponent from './CoursesComponent.vue'
import BooksComponent from './BooksComponent.vue'
export default {
    name:'MainComponent',

    components:{
        PanoramaComponent,
        CoursesComponent,
        BooksComponent,
        
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

  button{
                border-radius: 5px;
                border-style: none;
                color: white;
                padding: 10px 50px;
                background-color: #20ac97;
                margin-top: 40px;
                &:hover{
                    background-color: #171520;
                }
            }

</style>