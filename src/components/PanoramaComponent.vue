<template>
    <div>
        <FeedbackComponent />
        <AboutMeComponent />
    </div>
  
</template>

<script>
import FeedbackComponent from './FeedbackComponent.vue'
import AboutMeComponent from './AboutMeComponent.vue'
export default {
    name:'PanoramaComponent',
    components:{
        FeedbackComponent,
        AboutMeComponent,


    }
}
</script>

<style scoped lang="scss">
    

</style>