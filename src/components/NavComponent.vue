<template>
  <nav>
    <img src="../assets/motivation/images/dark-logo.png" alt="dark-logo">
    <ul>
        <li>
            <a href="#">Home<span>&#9660;</span></a>
        </li>
        <li>
            <a href="#">Pages<span>&#9660;</span></a>
        </li>
        <li>
            <a href="#">Courses<span>&#9660;</span></a>
        </li>
        <li>
            <a href="#">Features<span>&#9660;</span></a>
        </li>
        <li>
            <a href="#">Blog<span>&#9660;</span></a>
        </li>
        <li>
            <a href="#">Shop<span>&#9660;</span></a>
        </li>
    </ul>

    <ul>
        <li>        
            <font-awesome-icon icon="fa-regular fa-star" />
        </li>
        <li>        
            <font-awesome-icon icon="fa-regular fa-star" />
        </li>
        <li>        
            <font-awesome-icon icon="fa-regular fa-star" />
        </li>
        <li>        
            <font-awesome-icon icon="fa-regular fa-star" />
        </li>

    </ul>
  </nav>
</template>

<script>
export default {
    name:'NavComponent',

}
</script>

<style scoped lang="scss">

    

    img{
        max-width: 200px;
    }

    nav{
        display: flex;
        justify-content: space-around;
        align-items: center;
        padding-top: 20px;
        
        ul{
            display: flex;
            list-style: none;
            text-decoration: none;
            // transform: translateY(+25%);
            li{
                padding: 0px 20px;
                color: #171520;
                a{
                    text-decoration: none;
                    // span:hover{
                    // }
                }
            }

            
        }
    }

</style>