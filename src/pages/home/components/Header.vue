 <template>
    <div class="header">
        <div class="header-left">
            <span class="iconfont back-icon">&#xe624;</span>
        </div>
        <div class="header-input">
            <span class="iconfont">&#xe632;</span>
            输入城市景点/游玩主题
        </div>
        <router-link to="/city">
            <div class="header-right">
                            {{this.city}}
                <span class="iconfont arrow-icon">&#xe715;</span>
            </div>
        </router-link>
    </div>
</template>

<script>
import {mapState} from 'vuex'
export default {
  name: 'HomeHeader',
  computed: {
      ...mapState(['city'])
  }
}
</script>

<style lang="stylus" scoped>
    @import '~styles/varibles.styl' 
    .header
        line-height $headerHeight
        display flex
        background $bgColor
        color #fff
        .header-left
            width .64rem
            float left
            .back-icon
                text-align center
                font-size .4rem
        .header-input
            padding-left .2rem
            flex 1
            margin-top .12rem
            line-height .64rem
            height .64rem
            background #fff
            border-radius .1rem
            color #ccc
        .header-right
            min-width 1.04rem
            padding 0 .1rem
            float right
            text-align center
            color #fff
            .arrow-icon
                font-size .24rem
                margin-left -.04rem

</style>
