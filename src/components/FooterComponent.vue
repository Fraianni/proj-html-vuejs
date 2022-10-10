<template>
    <div class="container">
        <div class="links">

            <ul>
                <h2>Address</h2>

                <li> <a href="#">382 NE AOSDO AOS OEO A, 39324 923</a> </li>
                <li> <a href="#">+1241235521 (9am-5pm asdasd sad )</a> </li>
                <li> <a href="#">supportofiso@gmail.com</a> </li>
                <li>             
                <font-awesome-icon icon="fa-brands fa-facebook" /> <font-awesome-icon icon="fa-brands fa-instagram" /> <font-awesome-icon icon="fa-brands fa-youtube" /> <font-awesome-icon icon="fa-brands fa-twitter " />

                </li>
            </ul>
        </div>
        <BackTopComponent />
    </div>
</template>

<script>
import BackTopComponent from '../components/BackTopComponent.vue'    
export default {
    name:'FooterComponent',
    components:{
        BackTopComponent,

    }
    
}
</script>

<style scoped lang="scss">
       @import '../style/variables.scss';

    .container{
        display: flex;
        justify-content: center;
        background-color: $vulcan;
        .links{
            width: 1400px;
            display: flex;
            justify-content: space-between;
            ul{
                display: flex;
                flex-direction: column;
                list-style-type: none;
                color: white;
                text-align: left;
                li{
                    margin: 20px 0px;
                    color: gray;

                    a{
                    color: gray;
                }
                }
                
            }
        }
    }
</style>