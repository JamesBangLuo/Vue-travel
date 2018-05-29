<template>
<div>
  <home-header></home-header>
  <home-swiper ></home-swiper>
  <home-icons ></home-icons>
  <home-recommend ></home-recommend>
  <home-weekend ></home-weekend>
</div>
</template>
<script>
import HomeHeader from './components/Header'
import HomeSwiper from './components/Swiper'
import HomeIcons from './components/Icons'
import HomeRecommend from './components/Recommend'
import HomeWeekend from './components/Weekend'
export default {
  name: 'Home',
  components: {
    HomeHeader: HomeHeader,
    HomeSwiper: HomeSwiper,
    HomeIcons: HomeIcons,
    HomeRecommend: HomeRecommend,
    HomeWeekend: HomeWeekend
  },
  data () {
    return {
      // swiperList: [],
      // iconList: [],
      // recommendList: [],
      // weekendList: []
    }
  }
  // methods: {
  //   getHomeInfo () {
  //     axios.get('/api/index.json')
  //       .then(this.getHomeInfoSucc)
  //   },
  //   getHomeInfoSucc (res) {
  //     res = res.data
  //     if (res.ret && res.data) {
  //       const data = res.data
  //       this.swiperList = data.swiperList
  //       this.iconLsit = data.iconLsit
  //       this.recommendList = data.recommendList
  //       this.weekendList = data.weekendList
  //     }
  //     console.log(res)
  //   }

  // },
  // mounted () {
  //   this.getHomeInfo()
  // }
}
</script>

<style scoped>
</style>
