<template>
  <div>
    <swiper :options="swiperOption">
      <swiper-slide class="swiper-slide" v-for="item in slide" :key="item.id">
        <img :src="item.url" alt="">
      </swiper-slide>
      <!-- 分页器 -->
      <div class="swiper-pagination" slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
  import "swiper/dist/css/swiper.css";
  import {swiper,swiperSlide} from "vue-awesome-swiper"; //局部引入
  export default {
    name: 'HomeSwiper',
    components: {
      swiper,
      swiperSlide
    },
    data() {
      return {
        slide: [
          {
            id: "1",
            url: "../../assets/one.jpg"
          },
          {
            id: "2",
            url: "../../assets/two.jpg"
          },
          {
            id: "3",
            url: "../../assets/three.jpg"
          },
          {
            id: "4",
            url: "../../assets/fhor.jpg"
          },
        ],
        swiperOption: {//swiper3
          autoplay: 3000,
          speed: 1000,
        }
      };
    },
    mounted() {

    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="less" scoped>
  .swiper-container {
    width: 100%;
    height: 800px;
    img{
      width: 100%;
      height: 100%;
    }
  }
</style>
