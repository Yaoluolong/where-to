<template>
  <a class="nav-link" v-bind:href="linkItem.url">
    <div class="nav-img">
      <img v-bind:src="linkItem.img">
    </div>
    <span class="nav-title">{{linkItem.title}}</span>
  </a>
</template>
<script>
export default {
  name: 'HomeLink',
  props: {
    linkItem: Object
  }
}
</script>
<style lang="stylus">
.nav
  &-link
    text-decoration none
    float left
    text-align center
    width 20%
    margin 0 auto
    display block
  &-img
    img
      width 1.1rem
  &-title
    display block
    color #333
    font-size 0.3rem
    line-height 0.6rem
</style>
