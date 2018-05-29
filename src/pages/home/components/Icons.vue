<template>
  <div class="icons">
    <swiper>
      <swiper-slide v-for="(page,index) of pages" :key="index">
        <div class="icon" v-for="item in page" :key='item.id'>
          <div class="icon-img">
            <img class="img-content" :src="item.imgUrl">
            <p>{{item.desc}}</p>
          </div>
        </div>
      </swiper-slide>
      <!-- <swiper-slide>
        <div class="icon" v-for="place in iconList" :key='place.id'>
          <div class="icon-img">
            <img class="img-content" src="place.imgurl">
            <p>{{place.desc}}</p>
          </div>
        </div>
      </swiper-slide> -->
        <div class="swiper-pagination"  slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
export default {
  name: 'HomeIcons',
  data () {
    return {
      // swiperOption: {}
      page: [{
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
  },
  computed: {
    pages () {
      const pages = []
      this.page.forEach((item, index) => {
        const page = Math.floor(index / 2)
        if (!pages[page]) {
          pages[page] = []
        }
        pages[page].push(item)
      })
      return pages
    }
  }
}
</script>

<style lang="stylus" scoped>
.icons
 overflow :hidden
 height :0
 padding-bottom :50%
.icon
  position :relative
  overflow :hidden
  float :left
  width :50%
  height :0
  padding-bottom :50%
.icon-img
    position :absolute
    top :0
    left :0
    right :0
    bottom :0.44rem
    padding:0.1rem
.img-content
    display :block
    margin : 0 auto
    height :100%
.icon-desc
    text-align :center
</style>
