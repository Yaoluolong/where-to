<template>
  <a class="wrap-content-link" :href="item.href">
    <div class="wrap-content-link-img">
      <img v-bind:src="item.img">
    </div>
    <div class="wrap-content-link-title">{{item.title}}</div>
    <slot name="describe"></slot>
    <slot name="price"></slot>
  </a>
</template>
<script>
export default {
  name: 'WrapContent',
  props: ['item'],
  data () {
    return {

    }
  }
}
</script>
<style lang="stylus">
.wrap-content-link
  text-decoration none
  float left
  text-align center
  display block
  width 50%
  margin-bottom 0.2rem
  &-img
    img
      height 2.2rem
      width 95%
      border-radius 6%
  &-title
    font-size 0.3rem
    color #333
    display block
  &-describe
    height 0.28rem
    overflow hidden
    text-overflow:ellipsis;
    white-space: nowrap;
    font-size 0.28rem
    color #757575
  &-price
    color #ff7400
    font-size 0.4rem
  &-title
  &-describe
  &-price
    margin-bottom 0.1rem
</style>
