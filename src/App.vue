<template>
  <div id="app">
    <HeaderComponent />
    <MainComponent :courses="courses" />
    <FooterComponent />
  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue'
import MainComponent from './components/MainComponent.vue'
import FooterComponent from './components/FooterComponent.vue'

export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainComponent,
    FooterComponent

  },
  
}
</script>

<style>
  *{
    margin: 0;
    box-sizing: border-box;
    padding: 0;
  }
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  
}
</style>
