<template>
  <nav>
    <img src="../assets/motivation/images/dark-logo.png" alt="dark-logo">
    <ul>
        <li>
            <a href="#">Home</a>
        </li>
        <li>
            <a href="#">Pages</a>
        </li>
        <li>
            <a href="#">Courses</a>
        </li>
        <li>
            <a href="#">Features</a>
        </li>
        <li>
            <a href="#">Blog</a>
        </li>
        <li>
            <a href="#">Shop</a>
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
        
        ul{
            display: flex;
            list-style: none;
            text-decoration: none;
            transform: translateY(+25%);
            li{
                margin-right: 10px;
                color: #171520;
                a{
                    text-decoration: none;
                }
            }

            
        }
    }

</style>