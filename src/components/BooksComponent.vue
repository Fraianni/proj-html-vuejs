<template>
  <div class="container">
    <div class="books">
        <div class="info">
            <p>BOOK STORE ONLINE</p>
            <h1>Be Alpha With <span>Wingman's Book</span></h1>
            <ul>
                <li> <span><font-awesome-icon icon="fa-solid fa-check" /></span> Help you understand yourself better</li>
                <li><span><font-awesome-icon icon="fa-solid fa-check" /></span> Revealing mature tips</li>
                <li><span><font-awesome-icon icon="fa-solid fa-check" /></span> Give the right advice</li>
                <li><span><font-awesome-icon icon="fa-solid fa-check" /></span> Fascinating examples of alpha men</li>
            </ul>
            <button>Get Free Ebook</button>
        </div>
        <div class="covers">
            <div class="book-real-man">
                <img src="../assets/motivation/images/product-book-10-400x400.jpg" alt="">
                <p>Alpha Man by Max Coach</p>
                <p><span>29.00$</span></p>
                <div class="menu">
                    <font-awesome-icon icon="fa-solid fa-magnifying-glass" />
                    <font-awesome-icon icon="fa-solid fa-heart" />
                    <font-awesome-icon icon="fa-solid fa-cart-shopping" />
                    <font-awesome-icon icon="fa-solid fa-signal" />


                </div>
            </div>
            <div class="book-alpha-man">
                <img src="../assets/motivation/images/product-book-11-400x400.jpg" alt="">
                <p>Real Man 4.0 by Max Coach</p>
                <p><span>39.00$</span></p>
                <div class="menu">
                    <font-awesome-icon icon="fa-solid fa-magnifying-glass" />
                    <font-awesome-icon icon="fa-solid fa-heart" />
                    <font-awesome-icon icon="fa-solid fa-cart-shopping" />
                    <font-awesome-icon icon="fa-solid fa-signal" />

                </div>
            </div>

        </div>
    </div>
  </div>
</template>

<script>
export default {
    name:'BooksComponent'
}
</script>

<style scoped lang="scss">
    .container{
        display: flex;
        justify-content: center;
        padding: 30px 0px;
        margin-top: 100px;
        .books{
            width: 1400px;
            display: flex;
            text-align: left;
            .info{
                display: flex;
                flex-direction: column;
                width: 40%;
                ul{
                    list-style-type: none;  
                    li{
                        margin: 30px 0px;
                    }
                }
                span{
                        color:#20ac97;
                    }
                h1{
                    margin: 30px 0px;
                    font-size: 3rem;

                }
                button{
                border-radius: 5px;
                border-style: none;
                color: white;
                padding: 10px;
                width: 60%;
                background-color: #20ac97;
                margin-top: 40px;
                &:hover{
                    background-color: #171520;
                }
            }
            
        }
        .covers{
            display: flex;
            text-align: center;
            font-size: 1.2rem;
            font-weight:bold;
            img{
                margin: 0px 10px;
                height: 80%;
            }
            p{
                margin-top: 20px;
                span{
                color: #20ac97;   
                }
            }
            >*{
                position: relative;
                &:hover .menu{
                    display: flex;
                }
                .menu{
                    position:absolute;
                    height: 50%;
                    right:60px;
                    top: 70px;
                    display: none;
                    flex-direction: column;
                    justify-content: space-between;
                    >*{
                        border-radius: 50%;
                        background-color: white;
                        padding: 10px;
                        &:hover{
                            color: red;
                        }
                    }
                }
            }
            
            
        }
     }
    }
</style>