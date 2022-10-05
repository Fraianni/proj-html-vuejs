<template>
    <div>
        <FeedbackComponent />
        <AboutMeComponent />
        <YouTubeComponent />
    </div>
  
</template>

<script>
import FeedbackComponent from './FeedbackComponent.vue'
import AboutMeComponent from './AboutMeComponent.vue'
import YouTubeComponent from './YouTubeComponent.vue'
export default {
    name:'PanoramaComponent',
    components:{
        FeedbackComponent,
        AboutMeComponent,
        YouTubeComponent


    }
}
</script>

<style scoped lang="scss">
    

</style>