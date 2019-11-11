<template>
  <div>
    <home-header></home-header>
    <home-swiper></home-swiper>
    <div>更改了</div>
  </div>
</template>

<script>
  import HomeHeader from "./components/Header"
  import HomeSwiper from "./components/Swiper"
  export default {
    name: 'Home',
    data () {
      return {

      }
    },
    components:{
      HomeHeader,
      HomeSwiper
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="less" scoped>
  *{
    margin: 0;
    padding: 0;
    list-style: none;
  }

</style>
