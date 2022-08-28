<script>
export default {
  onLaunch: function () {
    console.log('App Launch')
  },
  onShow: function () {
    console.log('App Show')
  },
  onHide: function () {
    console.log('App Hide')
  },
  onLoad: function () {
    console.log('App onload')
    setTimeout(()=>{
      console.log('eeeeeee');
    },500)
  },
}
</script>

<!--<style lang="scss">-->
<style>
/*每个页面公共css */
/*@import '@/wxcomponents/vant/dist/common/index.wxss';*/

/*@font-face {*/
/*  font-family: 'iconfont';  !* project id 744578 *!*/
/*  src: url('//at.alicdn.com/t/font_744578_6p0r42ygi2o.eot');*/
/*  src: url('//at.alicdn.com/t/font_744578_6p0r42ygi2o.eot?#iefix') format('embedded-opentype'),*/
/*  url('//at.alicdn.com/t/font_744578_6p0r42ygi2o.woff2') format('woff2'),*/
/*  url('//at.alicdn.com/t/font_744578_6p0r42ygi2o.woff') format('woff'),*/
/*  url('//at.alicdn.com/t/font_744578_6p0r42ygi2o.ttf') format('truetype'),*/
/*  url('//at.alicdn.com/t/font_744578_6p0r42ygi2o.svg#iconfont') format('svg');*/
/*}*/
.iconfont {
  font-family: 'iconfont' !important;
  font-size: 16px;
  font-style: normal;
  -webkit-font-smoothing: antialiased;
  -webkit-text-stroke-width: 0.2px;
  -moz-osx-font-smoothing: grayscale;
}
</style>
