<template>
    <div class="container">
        <div class="about_me">
            <div class="alpha">
                <p>ABOUT ME</p>
                <h1>How to Be an Alpha Male: The 15 Habits of True Alphas</h1>
            </div>
            <div class="alpha_description">
                <p class="title"> Want to learn how to be <span>an alpha male</span>? How to be more masculine? How to be the man you've always wanted to be?</p>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Officiis consequuntur velit dolores ut, suscipit reiciendis quos minima doloribus hic quibusdam soluta autem, doloremque recusandae adipisci architecto, nihil inventore vel enim!</p>
            </div>
        </div>
    </div>

 
</template>

<script>
export default {
    name:'AboutMeComponent'
}
</script>

<style scoped lang="scss">
    .container{
        display: flex;
        justify-content: center;
    }
    
    .about_me{
        max-width: 1400px;
        display: flex;
        justify-content: space-between;
        margin-top: 100px;
        text-align: left;

        .alpha{
            max-width: 500px;
            margin-right: 200px;

            h1{
                font-size:2.9rem;
                margin-top: 20px;
            }
            p{
                color: #20ac97;
            }
        }
        .alpha_description{
            display: flex;
            flex-direction: column;
            justify-content: space-around;
           
            .title{
                font-weight: bold;
                span{
                    color:#20ac97

                }
            }
        }
    }

</style>