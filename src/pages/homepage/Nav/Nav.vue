<template>
  <div class="nav">
    <div class="link">
      <home-link v-for="(item ,index) of linkList" :key="index" :linkItem="item"></home-link>
    </div>
  </div>
</template>
<script>
import HomeLink from './components/Link'
export default {
  name: 'Nav',
  components: {
    HomeLink
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
        },
        {
          url: 'javascript:;',
          img: '//s.qunarzz.com/homenode/images/touchheader/group.png',
          title: '特惠酒店'
        },
        {
          url: 'javascript:;',
          img: '//s.qunarzz.com/homenode/images/touchheader/bargainflight.png',
          title: '低价机票'
        },
        {
          url: 'javascript:;',
          img: '//s.qunarzz.com/homenode/images/touchheader/inn.png',
          title: '低价机票'
        },
        {
          url: 'javascript:;',
          img: '//s.qunarzz.com/homenode/images/touchheader/haiwai.png',
          title: '海外酒店'
        },
        {
          url: 'javascript:;',
          img: '//s.qunarzz.com/homenode/images/touchheader/kezhan.png',
          title: '民宿'
        },
        {
          url: 'javascript:;',
          img: '//s.qunarzz.com/homenode/images/touchheader/bus.png',
          title: '汽车票船票'
        },
        {
          url: 'javascript:;',
          img: '//s.qunarzz.com/homenode/images/touchheader/tuan.png',
          title: '旅游团购'
        },
        {
          url: 'javascript:;',
          img: '//s.qunarzz.com/homenode/images/touchheader/freeTravel.png',
          title: '自由行'
        },
        {
          url: 'javascript:;',
          img: '//s.qunarzz.com/homenode/images/touchheader/car.png',
          title: '专车自驾'
        },
        {
          url: 'javascript:;',
          img: '//s.qunarzz.com/homenode/images/touchheader/aroundtravel.png',
          title: '周边短途'
        },
        {
          url: 'javascript:;',
          img: '//s.qunarzz.com/homenode/images/touchheader/jr.png',
          title: '金融理财'
        },
        {
          url: 'javascript:;',
          img: '//s.qunarzz.com/homenode/images/touchheader/card.png',
          title: '保险车险'
        },
        {
          url: 'javascript:;',
          img: '//s.qunarzz.com/homenode/images/touchheader/travel.png',
          title: '攻略'
        },
        {
          url: 'javascript:;',
          img: '//s.qunarzz.com/homenode/images/touchheader/youlun.png',
          title: '邮轮'
        },
        {
          url: 'javascript:;',
          img: '//s.qunarzz.com/homenode/images/touchheader/oversea.png',
          title: '换外币'
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
    a:nth-child(-n+5)
      .nav-img
        img
          width 1rem
</style>
