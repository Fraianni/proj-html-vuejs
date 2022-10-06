<template>
  <div class="container">
    
    <div class="courses">
        
        <div class="course" v-for="course in courses" :key="course.thumb">
            <CourseComponent :course="course"/>
        </div>
    </div>
  </div>
</template>

<script>
import CourseComponent from './CourseComponent.vue'
export default {
    name:'CoursesComponent',
    components:{
        CourseComponent,
    },
    props:{
        courses:Array,

    }
}
</script>

<style scoped lang="scss">
    .container{
        display: flex;
        justify-content: center;
        padding-bottom: 50px;
        .courses{
            width: 1400px;
            display: flex;
            flex-wrap: wrap;
            
            .course{
                // display: inline-block;
                width: calc(100% / 3 ) ;
                &:hover{
                    transform: scale(1.1); 
                    opacity: 0.9;
                }
            }
        }
    }

</style>