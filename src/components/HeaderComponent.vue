<template>
    <header>
        <NavComponent/>
        <HeroHeaderComponent/>
        

    </header>
  
</template>

<script>
import NavComponent from '../components/NavComponent.vue'
import HeroHeaderComponent from '../components/HeroHeaderComponent.vue'

export default {
    name:'HeaderComponent',

    components:{
        NavComponent,
        HeroHeaderComponent,


    }

}
</script>

<style scoped lang="scss">
    header{
        background-image: url('../assets/motivation/images/background-pattern-wavify.png');
    }

</style>