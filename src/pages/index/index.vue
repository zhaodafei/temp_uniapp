<template>
  <view class="content">
    <!--<image class="logo"  src="/static/logo.png"></image>-->
    <!--<view class="text-area">
      <text class="title" :class="title">{{ title }}</text>
    </view>-->

    <!--<view>
      <text class="title"> sssssss启动遇到报错,就是你的版本有问题,或者少依赖 </text>
    </view>-->
    <!--轮播图-->
    <view>
      <swiper class="banners" indicator-dots indicator-color='ivory' indicator-active-color='#d43c33'>
        <swiper-item v-for="(item,index) in bannerList" :key="index">
          <image :src="item.pic" />
        </swiper-item>
      </swiper>
    </view>

    <!-- 热门榜 -->
    <view class="page-hot">
      <view class="hot-header">
        <text class="title">精彩内容</text>
        <text class="link" @tap="toHotPage">查看更多</text>
      </view>

      <view class="hot-content">
        <view class="img-list" v-for="(item,index) in hotList" :key="index">
          <image :src="item.pic"/>
        </view>
      </view>
    </view>

    <view class="page-recommend">
      <view class="recommend-header">
        <text class="title">精彩内容 wwwwww</text>
        <text class="link" @tap="toRecommendPage">查看更多</text>
      </view>
      <view>
        <text>sssssss</text>
      </view>

      <!--<view class="hot-content">
        <view class="img-list" v-for="(item,index) in recommendList" :key="index">
          <image :src="item.pic"/>
        </view>
      </view>-->
    </view>

  </view>
</template>

<script setup>
import {ref} from 'vue'
// import {onLaunch, onShow, onHide, onLoad} from '@dcloudio/uni-app'
import bannerImg from '@/static/img/fei01.jpg'

const title = ref('大飞Vue3,uni-appddd启动成功了');
const bannerList = ref([
  {pic: bannerImg},
  {pic: bannerImg},
  {pic: bannerImg},
])

const hotList = ref([
  {pic: bannerImg},
  {pic: bannerImg},
  {pic: bannerImg},
  {pic: bannerImg},
])

const recommendList = ref([
  {pic: bannerImg},
  {pic: bannerImg},
  {pic: bannerImg},
  {pic: bannerImg},
  {pic: bannerImg},
  {pic: bannerImg},
])

const toHotPage = () => {}
const toRecommendPage = () => {}

</script>


<style lang="scss">
.page-hot{
  padding: 0 16rpx;

  .hot-header {
    display: flex;
    align-items: center;
    justify-content: space-between;

    .title, .link {
      font-size: 32rpx;
      color: #000;
      font-weight: bold;
    }
  }

  .hot-content {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    padding-bottom: 12rpx;
    margin-left: -8rpx;
    margin-right: -8rpx;

    .img-list {
      width: 50%;
      padding: 0 8rpx;
      margin-bottom: 16rpx;
      box-sizing: border-box;
      image {
        width: 100%;
        height: 200rpx;
        border-radius: 8rpx;
        vertical-align: top;
        background-color: #c0c0c0;
      }
    }
  }
}

.page-recommend{
  padding: 0 16rpx;

  .hot-header {
    display: flex;
    align-items: center;
    justify-content: space-between;

    .title, .link {
      font-size: 32rpx;
      color: #000;
      font-weight: bold;
    }
  }
}
</style>
