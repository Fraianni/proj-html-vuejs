<template>
  <div class="container">
      <div class="icons">
        <div class="icon" v-for="icon in client" :key="icon.thumb">
          <img :src="require(`@/assets/motivation/images/${icon.thumb}`)" alt="">
        </div>
      </div>
  </div>
</template>

<script>
export default {
    name:'ClientComponent',
    props:{
      client:Array,

    }
}
</script>

<style scoped lang="scss">
  .container{
    display: flex;
    justify-content: center;
    margin-top: 100px;
    padding-bottom: 100px;
    .icons{
      width: 1400px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      .icon{
        filter: grayscale(0.9);
      }
    }
  }
</style>