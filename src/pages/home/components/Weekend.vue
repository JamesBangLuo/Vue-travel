<template>
    <div>
        <div class="weekend-title">周末去哪儿</div>
        <ul>
            <li class="item" border-bottom v-for=" item in weekendList" :key="item.id">
                <div class="item-img-wrappers">
                <img :src="item.imgUrl" class="item-img">
                <div class="item-info">
                    <p class="item-title">{{item.title}}</p>
                    <p class="item-desc">{{item.desc}}</p>
                </div>
                </div>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
  name: 'HomeWeekend',
  //   props: {
  //     list: Array
  //   }
  data () {
    return {weekendList: [{
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
    }]}
  }

}
</script>

<style lang="stylus" scoped>
.weekend-title
    line-height :0.8rem
    background :#eee
    text-indent :0.2rem
    text-align :left
.item-img-swappers
        overflow :hidden
        height  :0
        padding-bottom :33.9%
.item-img
        width :100%
.item-info
        padding :0.1rem
        text-align :left
.item-title
        line-hec0c0c0ight :0.54rem
        font-size :0.32rem
.item-desc
        color :#c0c0c0
        line-height :0.54rem
</style>
