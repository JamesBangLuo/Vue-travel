<template>
    <div class="wrapper">
    <swiper :options="swiperOption">
    <!-- slides -->
    <swiper-slide v-for="item of swiperList" :key="item.id">
      <img class="swiper-img" :src="item.imgUrl"/>
      </swiper-slide>
    <div class="swiper-pagination"  slot="pagination"></div>
  </swiper>
   </div>
</template>

<script>
export default {
  name: 'HomeSwiper',
  data () {
    return { swiperOption: {
      pageination: '.swiper-pagination',
      loop: true,
      autoplay: true
    },
    swiperList: [{
      id: '0001',
      imgUrl: 'https://imgs.qunarzz.com/p/tts5/1803/52/f0bdeb873d1a3402.jpg_r_390x260x90_e9ac2738.jpg'
    }, {
      id: '0002',
      imgUrl: 'https://imgs.qunarzz.com/p/tts5/1803/52/f0bdeb873d1a3402.jpg_r_390x260x90_e9ac2738.jpg'
    }, {
      id: '0003',
      imgUrl: 'https://imgs.qunarzz.com/p/tts5/1803/52/f0bdeb873d1a3402.jpg_r_390x260x90_e9ac2738.jpg'
    }, {
      id: '0004',
      imgUrl: 'https://imgs.qunarzz.com/p/tts5/1803/52/f0bdeb873d1a3402.jpg_r_390x260x90_e9ac2738.jpg'
    }]
    }
  }
  // computed: {
  //   showSwiper () {
  //     return this.list.length
  //   }
  // }
}
</script>
<style lang='stylus' scoped>
  .wrapper
    overflow :hidden
    width :100%
    height :0
    padding-bottom :31.25%
  .swiper-img
   width :100%
</style>
