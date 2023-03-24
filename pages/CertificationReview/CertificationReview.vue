<template>
	<view class="review">
		<image class="review_img" src="../../static/img/shenheing.png" mode=""></image>
		<view class="review_yes">
			提交成功
		</view>
		<view class="review_text">
			后台审核，请耐心等候结果
		</view>
		<view class="re">
			返回
		</view>
	</view>
</template>

<script>
</script>

<style>
	.review{
		height: 1264rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		position: relative;
	}
	.review_img{
		width: 654rpx;
		height: 410rpx;
		margin: 62rpx 48rpx 40rpx 48rpx;
	}
	.review_yes{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 38rpx;
		text-align: center;
	}
	.review_text{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
		line-height: 33rpx;
		margin-top: 16rpx;
		text-align: center;
	}
	.re{
		position: absolute;
		bottom: 0;
		margin: 0 30rpx 16rpx 30rpx;
		width: 690rpx;
		height: 88rpx;
		background: #3891ED;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #FFFFFF;
		line-height: 88rpx;
		text-align: center;
	}
</style>