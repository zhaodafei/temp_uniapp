<template>
	<view class="content">
		<image class="logo" src="/static/logo.png"></image>
		<view>
			<text class="title">{{title}} sss</text>
		</view>
    <view>
      <text class="title"> 启动遇到报错,就是你的版本有问题,或者少依赖 </text>
    </view>
    <view>
      <van-button type="primary">主要按钮</van-button>
      <van-switch active-color="#07c160" inactive-color="#ee0a24" />
    </view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: '大飞,uni-app启动成功了'
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style>
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.logo {
		height: 200rpx;
		width: 200rpx;
		margin: 200rpx auto 50rpx auto;
	}

	.text-area {
		display: flex;
		justify-content: center;
	}

	.title {
		font-size: 36rpx;
		color: #8f8f94;
	}
</style>
