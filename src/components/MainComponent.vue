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
    <ClientComponent :client="client" />
    <SliderComponent :slides="slides" />
    <div class="articles-titles">
      <div class="titles">
        <p>BLOG UPDATED</p>
        <h1>Interesting <span>articles updated</span> daily</h1>
      </div>
    </div>
    <ArticlesComponent :articles="articles" />
    <p class="view"> <a href="#">VIEW ALL POSTS</a> </p>

     
  </main>
</template>

<script>
import courses from '../assets/data/courses.json'
import client from '../assets/data/client.json'
import slides from '../assets/data/slides.json'
import articles from '../assets/data/articles.json'
import PanoramaComponent from './PanoramaComponent.vue'
import CoursesComponent from './CoursesComponent.vue'
import BooksComponent from './BooksComponent.vue'
import ClientComponent from './ClientComponent.vue'
import SliderComponent from './SliderComponent.vue'
import ArticlesComponent from './ArticlesComponent.vue'

export default {
    name:'MainComponent',

    components:{
    PanoramaComponent,
    CoursesComponent,
    BooksComponent,
    ClientComponent,
    SliderComponent,
    ArticlesComponent,
},
   
    data(){
    return {
      courses,
      client,
      slides,
      articles
    }
  }
}
</script>

<style scoped lang="scss">
   @import '../style/variables.scss';
  .courses-titles{
    margin: 50px 0px;
    h3{
      color: gray;
    }
    span{
      color:$green_header;
    }
  }

  .articles-titles{
    display: flex;
    justify-content: center;
    margin-top: 100px;
    .titles{
      width: 1400px;

      text-align: left;
    }
    .p{
      color: gray;
    }
    span{
      color:$green_header;
    }
  }

  .view{
      margin-top: 50px;
      margin-bottom: 200px;
      a{
        color:$green_header;

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