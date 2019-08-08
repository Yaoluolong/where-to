<template>
  <div class="wrap">
    <wrap-title>
      <template v-slot:switchBtn>
        <a
          href="javascript:;"
          v-for="(item,index) of buttonList[0]"
          :key="'buttonList[0]'+index"
          @click="cursor.splice(0,1,index)"
          :class="{active:cursor[0]==index}"
        >{{item}}</a>
      </template>
      <template v-slot:more>
        <a href="javascript:;">
          <span>更多</span>
          <span class="iconfont">&#xe633;</span>
        </a>
      </template>
    </wrap-title>
    <div class="wrap-content">
      <wrap-content
        v-for="(item,index) of wrapContentList[cursor[0]]"
        :key="index"
        :item="item"
      >
      <template v-slot:describe>
        <div class="wrap-content-link-describe">{{item.describe}}</div>
      </template>
      <template v-slot:price>
        <div class="wrap-content-link-price">¥{{item.price}}<span style="font-size:0.3em;margin-left:0.1rem">起</span></div>
      </template>
      </wrap-content>
    </div>

  </div>
</template>
<script>
import WrapTitle from './components/Title'
import WrapContent from './components/Content'
export default {
  components: {
    WrapTitle,
    WrapContent
  },
  data () {
    return {
      cursor: [0],
      buttonList:
      [
        ['今日特惠', '特惠门票', '特惠一日游'],
        ['趣味亲子游', '毕业旅行在路上']
      ],
      wrapContentList:
      [
        [
          {
            href: 'javascript',
            img: '//imgs.qunarzz.com/p/tts5/1810/84/88bd71ec1ca69602.jpg_r_480x320x90_6927085e.jpg',
            title: '福州-云南 5天跟团游',
            describe: '新升级+不夜宿火车丨丽江大理丨海景温泉（西双版纳/香格里拉/泸沽湖）随心组合',
            price: '1850'
          },
          {
            href: 'javascript',
            img: '//imgs.qunarzz.com/p/tts5/1810/84/88bd71ec1ca69602.jpg_r_480x320x90_6927085e.jpg',
            title: '福州-云南 5天跟团游',
            describe: '新升级+不夜宿火车丨丽江大理丨海景温泉（西双版纳/香格里拉/泸沽湖）随心组合',
            price: '1850'
          },
          {
            href: 'javascript',
            img: '//imgs.qunarzz.com/p/tts5/1810/84/88bd71ec1ca69602.jpg_r_480x320x90_6927085e.jpg',
            title: '福州-云南 5天跟团游',
            describe: '新升级+不夜宿火车丨丽江大理丨海景温泉（西双版纳/香格里拉/泸沽湖）随心组合',
            price: '1850'
          },
          {
            href: 'javascript',
            img: '//imgs.qunarzz.com/p/tts5/1810/84/88bd71ec1ca69602.jpg_r_480x320x90_6927085e.jpg',
            title: '福州-云南 5天跟团游',
            describe: '新升级+不夜宿火车丨丽江大理丨海景温泉（西双版纳/香格里拉/泸沽湖）随心组合',
            price: '1850'
          }
        ],
        [
          {
            href: 'javascript',
            img: '//imgs.qunarzz.com/p/tts5/1810/84/88bd71ec1ca69602.jpg_r_480x320x90_6927085e.jpg',
            title: '福州-云南 5天跟团游',
            describe: '新升级+不夜宿火车丨丽江大理丨海景温泉（西双版纳/香格里拉/泸沽湖）随心组合',
            price: '1850'
          },
          {
            href: 'javascript',
            img: '//imgs.qunarzz.com/p/tts5/1810/84/88bd71ec1ca69602.jpg_r_480x320x90_6927085e.jpg',
            title: '福州-云南 5天跟团游',
            describe: '新升级+不夜宿火车丨丽江大理丨海景温泉（西双版纳/香格里拉/泸沽湖）随心组合',
            price: '1850'
          },
          {
            href: 'javascript',
            img: '//imgs.qunarzz.com/p/tts5/1810/84/88bd71ec1ca69602.jpg_r_480x320x90_6927085e.jpg',
            title: '福州-云南 5天跟团游',
            describe: '新升级+不夜宿火车丨丽江大理丨海景温泉（西双版纳/香格里拉/泸沽湖）随心组合',
            price: '1850'
          },
          {
            href: 'javascript',
            img: '//imgs.qunarzz.com/p/tts5/1810/84/88bd71ec1ca69602.jpg_r_480x320x90_6927085e.jpg',
            title: '福州-云南 5天跟团游',
            describe: '新升级+不夜宿火车丨丽江大理丨海景温泉（西双版纳/香格里拉/泸沽湖）随心组合',
            price: '1850'
          }
        ],
        [
          {
            href: 'javascript',
            img: '//imgs.qunarzz.com/p/tts5/1810/84/88bd71ec1ca69602.jpg_r_480x320x90_6927085e.jpg',
            title: '福州-云南 5天跟团游',
            describe: '新升级+不夜宿火车丨丽江大理丨海景温泉（西双版纳/香格里拉/泸沽湖）随心组合',
            price: '1850'
          },
          {
            href: 'javascript',
            img: '//imgs.qunarzz.com/p/tts5/1810/84/88bd71ec1ca69602.jpg_r_480x320x90_6927085e.jpg',
            title: '福州-云南 5天跟团游',
            describe: '新升级+不夜宿火车丨丽江大理丨海景温泉（西双版纳/香格里拉/泸沽湖）随心组合',
            price: '1850'
          },
          {
            href: 'javascript',
            img: '//imgs.qunarzz.com/p/tts5/1810/84/88bd71ec1ca69602.jpg_r_480x320x90_6927085e.jpg',
            title: '福州-云南 5天跟团游',
            describe: '新升级+不夜宿火车丨丽江大理丨海景温泉（西双版纳/香格里拉/泸沽湖）随心组合',
            price: '1850'
          },
          {
            href: 'javascript',
            img: '//imgs.qunarzz.com/p/tts5/1810/84/88bd71ec1ca69602.jpg_r_480x320x90_6927085e.jpg',
            title: '福州-云南 5天跟团游',
            describe: '新升级+不夜宿火车丨丽江大理丨海景温泉（西双版纳/香格里拉/泸沽湖）随心组合',
            price: '1850'
          }
        ]
      ]
    }
  },
  creat () {
    this.cursor.splice(0, this.buttonList.length, 0)
  }
}

</script>
<style lang="stylus">
.wrap
  &-content
    margin 0.1rem 0.1rem
</style>
