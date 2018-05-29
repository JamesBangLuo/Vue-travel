<template>
    <div>
        <div class="recommand-title">热销推荐</div>
        <ul>
            <li class="item" border-bottom v-for="item in weekendList" :key="item.id">
                <img :src="item.imgUrl" class="item-img">
                <div class="item-info">
                    <p class="item-title">{{item.title}}</p>
                    <p class="item-desc">{{item.desc}}</p>
                    <button class="item-button">查看详情</button>
                </div>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
  name: 'HomeRecommend',
  data () {
    return {
      weekendList: [{
        id: '0001',
        imgUrl: 'https://imgs.qunarzz.com/p/tts5/1803/52/f0bdeb873d1a3402.jpg_r_390x260x90_e9ac2738.jpg',
        title: '北京',
        desc: '温泉'
      }, {
        id: '0002',
        imgUrl: 'https://imgs.qunarzz.com/p/tts5/1803/52/f0bdeb873d1a3402.jpg_r_390x260x90_e9ac2738.jpg',
        title: '北京',
        desc: '景点'
      }, {
        id: '0003',
        imgUrl: 'https://imgs.qunarzz.com/p/tts5/1803/52/f0bdeb873d1a3402.jpg_r_390x260x90_e9ac2738.jpg',
        title: '北京',
        desc: '庙宇'
      }]
    }
  }
//   props: {
//     list: Array
//   }
}
</script>

<style lang="stylus" scoped>
.recommand-title
    line-height :0.8rem
    background :#eee
    text-indent :0.2rem
    text-align :left
.item
    display :flex
    overflow :hidden
    height :1.9rem
.item-img
    width :4rem
    width :4rem
    height :1.7rem
    padding-bottom :0.1rem
.item-info
    flex :1
    padding :0.1rem
    text-align :left
.item-title
    line-hec0c0c0ight :0.54rem
    font-size :0.32rem
.item-desc
    color :#c0c0c0
    line-height :0.54rem
.item-button
    line-height :0.44rem
    margin-top :0.1rem
    background :#ff9300
    padding :0.1rem
    border-radius :0.2rem
</style>
