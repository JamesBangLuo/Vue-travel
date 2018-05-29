<template>
  <ul class="list">
    <!-- <li class="item" v-for="item of letters" :key="item" :ref="item" >
      {{item}}
    </li> -->
  </ul>
</template>

<script>
export default {
  name: 'CityAlphabet',
  props: {
    cities: Object
  }
}
</script>

<style lang="stylus" scoped>
 .list
    display :flex
    flex-direction :column
    position :absolute
    justify-content :center
    right :0
    top: 1.58rem
    bottom :0
    width :.4rem
 .item
    line-height :.4rem
    text-align :center
</style>
