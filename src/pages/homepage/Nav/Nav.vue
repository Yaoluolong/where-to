<template>
  <div class="nav">
    <div class="link">
      <home-link v-for="(item ,index) of linkList" :key="index" :linkItem="item"></home-link>
    </div>
    <home-line>

    </home-line>
  </div>
</template>
<script>
import HomeLink from './components/Link'
import HomeLine from './components/Line'
export default {
  name: 'Nav',
  components: {
    HomeLink,
    HomeLine
  },
  data () {
    return {
      linkList: [
        {
          url: 'javascript:;',
          img: '//s.qunarzz.com/homenode/images/touchheader/hotel.png',
          title: '酒店'
        },
        {
          url: 'javascript:;',
          img: '//s.qunarzz.com/homenode/images/touchheader/flight.png',
          title: '机票'
        },
        {
          url: 'javascript:;',
          img: '//s.qunarzz.com/homenode/images/touchheader/package.png',
          title: '度假'
        },
        {
          url: 'javascript:;',
          img: '//s.qunarzz.com/homenode/images/touchheader/train.png',
          title: '火车票'
        },
        {
          url: 'javascript:;',
          img: '//s.qunarzz.com/homenode/images/touchheader/piao.png',
          title: '景点门票'
        }
      ],
      lineList: [
        {
          url: 'javascript:;',
          img: '//s.qunarzz.com/homenode/images/touchheader/hotel.png',
          title: '酒店'
        }
      ]
    }
  }
}
</script>
<style lang="stylus">
.nav
  margin 0.15rem 0
  width 100%
  text-align center
  .link
    &:after
      content ''
      display block
      clear both
</style>
