<template>
 <div class="header">城市选择
   <router-link to="/">
     <div class="iconfont header-back">&#xe624;</div>
   </router-link>
 </div>
</template>

<script>
export default {
  name: 'CityHeader'
}
</script>

<style lang="stylus" scoped>
.header
 position :relative
 overflow :hidden
 height :.86rem
 line-height :.86rem
 color :#fff
 text-align :center
 background :#0080ff
.header-back
 position :absolute
 top :0
 left :0
 font-size :0.4rem
 width :0.64rem
 color :#ffffff
</style>
