<template>
    <div class="header">
      <div class="header-left"><img src="//s.qunarzz.com/homenode/images/logo_camel.png"></div>
      <div class="header-center">去哪儿旅行</div>
      <div class="header-right"><span class="iconfont">&#xe64e;</span></div>
    </div>
</template>
<script>
export default {
  name: 'HomeHeader'
}
</script>
<style lang="stylus">
.header
  display flex
  line-height 0.8rem
  color #333
  &-left
    margin-left 0.2rem
    float left
    text-align center
    img
      vertical-align middle
      width 0.8rem
  &-center
    flex 1
    margin-left 0.25rem
    font-size 0.4rem
    padding-top 0.15rem
  &-right
    float right
    width 1rem
    text-align center
    span
      font-size 0.7rem
</style>
