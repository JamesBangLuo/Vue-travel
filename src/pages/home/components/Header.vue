<template>
<div class="header">
  <div class="header-left">
    <span class="iconfont">&#xe624;</span>
  </div>
  <div class="header-input">
    <span class="iconfont">&#xe632;</span>
    输入景点</div>
    <router-link to="./city">
  <div class="header-right">深圳
    <span class="iconfont">&#xe64a;</span>
  </div>
    </router-link>
</div>
</template>
<script>
export default {
  name: 'HomeHeader'
}
</script>

<style lang="stylus" scoped>
  @import '~styles/varibles.styl'
  .header
    display :flex
    line-height: 0.86rem
    background: $bgColor
    color: #fff
    .header-left
     width: 0.64rem
     float: left
    .header-input
     flex:1
     line-height :0.64rem
     height :0.64rem
     margin-top :0.12rem
     margin-left:0.2rem
     background :#fff
     border-radius :0.1rem
     color:#ccc
    .header-right
     width: 1.24rem
     float: right
     text-align :center
     color :#000000

</style>
