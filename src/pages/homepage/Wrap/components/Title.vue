<template>
  <div class="wrap-title">
    <div class="wrap-title-left">
      <slot name="switchBtn"></slot>
    </div>
    <div class="wrap-title-right">
        <slot name="more"></slot>
    </div>
  </div>
</template>
<script>
export default {
  name: 'WrapTitle'
}
</script>
<style lang="stylus">
.wrap-title
  margin-left 0.15rem
  a
    text-decoration none
    color #333
  &-left
    display flex
    flex 1
    float left
    align-items center
    margin-top 0.03rem
    font-size 14px
    a
      font-size 0.2rem
      padding 0.2rem 0.2rem
      border 0.02rem solid #cacaca
      border-radius 7%
      display inline-block
      margin 0 0.05rem
    .active
      background #3bb0d0
      color #ffffff
  &-right
    float right
    a
      span
        font-size 0.1rem
        display block
        line-height 0.75rem
        float left
        padding-right 0.1rem
  &:after
    content ''
    display block
    clear both
</style>
