<template>
  <nav>
    <img src="../assets/motivation/images/dark-logo.png" alt="dark-logo">
    <ul>
        <li>
            <div class="dropdown">
                <a href="#">Home<span>&#9660;</span></a>

                <div class="dropdown-content">
                    <div class="links">
                        <a href="#">Link 1</a>
                        <a href="#">Link 2</a>
                        <a href="#">Link 3</a>
                        <a href="#">Link 1</a>
                        <a href="#">Link 2</a>
                        <a href="#">Link 3</a>
                        <a href="#">Link 1</a>
                        <a href="#">Link 2</a>
                        <a href="#">Link 3</a>
                    </div>
                    <div class="links">
                        <a href="#">Link 1</a>
                        <a href="#">Link 2</a>
                        <a href="#">Link 3</a>
                        <a href="#">Link 1</a>
                        <a href="#">Link 2</a>
                        <a href="#">Link 3</a>
                        <a href="#">Link 1</a>
                        <a href="#">Link 2</a>
                        <a href="#">Link 3</a>
                    </div>
                    <img src="../assets/motivation/images/homepages-mega-menu-image-alt.jpg" alt="">
                </div>
            </div>
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
            <!-- <font-awesome-icon icon="fa-solid fa-check" /> -->
            <font-awesome-icon icon="fa-brands fa-facebook" />
        </li>
        <li>        
            <font-awesome-icon icon="fa-brands fa-instagram" />
        </li>
        <li>        
            <font-awesome-icon icon="fa-brands fa-youtube" />
        </li>
        <li>        
            <font-awesome-icon icon="fa-brands fa-twitter " />
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

    .dropdown-content {
        display: none;
        position: absolute;
        left: 18%;
        background-color: #f9f9f9;
        min-width: 1200px;
        box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
        z-index: 1;
        padding: 50px;
        .links{
            display: flex;
            flex-direction: column;
        }
        img{
            width: 600px;
        }
    }

    .dropdown:hover .dropdown-content {
        display: flex;
        justify-content: space-between;
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