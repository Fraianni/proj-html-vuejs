<template>
    <div class="container">
        
        <div class="articles">
            <div class="post" v-for="article in articles" :key="article.id">
                <img :src="require(`@/assets/motivation/images/${article.thumb}`)" alt="">
                <p class="date"> <font-awesome-icon icon="fa-regular fa-calendar" /> {{article.date}}</p>
                <p class="title">{{article.title}}</p>
                <p class="description">{{article.description}}</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:'AritclesComponent',
    props:{
        articles:Array,
    }
}
</script>

<style scoped lang="scss">
    @import '../style/variables.scss';
    .container{
        display: flex;
        justify-content: center;
        margin-top: 100px;
        .articles{
            width: 1400px;
            display: flex;
            justify-content: space-between;
            .post{
                text-align: left;
                max-width: calc(100% / 4 -20px);
                margin: 10px;
                img{
                    width: 100%;
                }
                p{
                    margin:10px 0px;
                }
                .date{
                    color:lightgray;
                }
                .description{
                    color:lightgray
                }
            }
        }
       
    }
</style>