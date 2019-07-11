 <template>
    <div>
        <div class="title">周末去哪儿</div>
        <ul>
            <li v-for="item of recommedList" 
                :key="item.id" 
                class="item border-buttom">
                <div class="item-img-wrapper">
                    <img :src="item.imgUrl" class="item-img" alt="">
                </div>
                <div class="item-info">
                    <p class="item-title">{{item.title}}</p>
                    <p class="item-desc">{{item.desc}}</p>
                </div>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
  name: 'HomeWeekend',
  data() {
      return {
          recommedList: [{
          id: '0001',
          imgUrl: 'http://img1.qunarzz.com/sight/p0/1409/19/adca619faaab0898245dc4ec482b5722.jpg_140x140_80f63803.jpg',
          title: '北京温泉排行榜',
          desc: '细数北京温泉，温暖你的冬天'
      },{
          id: '0002',
          imgUrl: 'http://img1.qunarzz.com/sight/p0/1409/19/adca619faaab0898245dc4ec482b5722.jpg_140x140_80f63803.jpg',
          title: '北京温泉排行榜',
          desc: '细数北京温泉，温暖你的冬天'
      },{
          id: '0003',
          imgUrl: 'http://img1.qunarzz.com/sight/p0/1409/19/adca619faaab0898245dc4ec482b5722.jpg_140x140_80f63803.jpg',
          title: '北京温泉排行榜',
          desc: '细数北京温泉，温暖你的冬天'
      },{
          id: '0004',
          imgUrl: 'http://img1.qunarzz.com/sight/p0/1409/19/adca619faaab0898245dc4ec482b5722.jpg_140x140_80f63803.jpg',
          title: '北京温泉排行榜',
          desc: '细数北京温泉，温暖你的冬天'
      },{
          id: '0005',
          imgUrl: 'http://img1.qunarzz.com/sight/p0/1409/19/adca619faaab0898245dc4ec482b5722.jpg_140x140_80f63803.jpg',
          title: '北京温泉排行榜',
          desc: '细数北京温泉，温暖你的冬天'
      }]
      }
  }
}
</script>

<style lang="stylus" scoped>
@import '~styles/mixins.styl'
.title
    margin-top: .2rem
    line-height: .8rem
    background: #eee
    text-indent: .2rem
.item-img-wrapper
    overflow hidden
    height 0
    padding-bottom 33.9%
    .item-img
        width: 100%
.item-info
    padding: .1rem
    min-width: 0
    .item-title
        line-height: .54rem
        font-size: .32rem
        ellipsis()
    .item-desc
        line-height: .4rem
        color: #ccc
        ellipsis()
</style>
