<template>
    <section>
        <div class="HeaderInfo">
            <h5>I'M WINGMAN</h5>
            <h1>Peace On Earth A Wonderful Wish But No Way</h1>
            <p>Succes is not overnight.It is when everyday you get a little better than the day before</p>
            <button> Get Started For &#8594;</button>
        </div>
        <img src="../assets/motivation/images/home-movation-hero-image.png" alt="">
    </section>
  
</template>

<script>
export default {
    name:'HeroHeaderComponent'
}
</script>

<style scoped lang="scss">
    section{
        display: flex;
        justify-content: space-around;
        align-items: center;
        margin-top: 100px;
        .HeaderInfo{
            max-width: 450px;
            text-align:left;
            font-size: 2rem;
        p{
            font-size: 1rem;
        }
        h5{
            font-size: 1rem;
        }
        button{
            border-radius: 5px;
            border-style: none;
            padding: 10px 50px;
            color: white;
            background-color: #20ac97;
        }
    }
    }

</style>