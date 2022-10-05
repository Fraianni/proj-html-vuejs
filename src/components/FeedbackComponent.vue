<template>
    <div class="container">
        <div class="feedback">
            <div class="stats">
                <h3>1.926</h3>
                <p>FINISHED SESSIONS</p>
            </div>
            <div class="stats">
                <h3>100%</h3>
                <p>SATISFACTION RATE</p>
            </div>
            <div class="stats">
                <h3>3092+</h3>
                <p>ENROLLED LEARNERS</p>
            </div>
            <div class="stats double">
                <h3>200</h3>
                <p>ONLINE ISTRUCTORS</p>
            </div>
        </div>
    </div>

 
    
  
</template>

<script>
export default {
    name:'FeedbackComponent'
}
</script>

<style scoped lang="scss">

    .container{
        display: flex;
        justify-content: center;
    }
    .feedback{
        width: 1400px;

        display: flex;
        justify-content: center;
        .stats{
            display: flex;
            flex-direction: column;
            height: 70px;
            justify-content:space-around;
            align-items: center;
            margin: 20px 0px;
            border-left:1px dashed #20ac97;
            padding: 0px 120px;
            &.double{
                border-right:1px dashed #20ac97;

            }

           
            h3{
                font-size: 2rem;
                color: #20ac97;
                margin-bottom: 0px;
                margin-top: 0px;
            }
            p{
                font-size: 0.7rem;
                transform: translateY(+25%);
            }
        }
    }

</style>