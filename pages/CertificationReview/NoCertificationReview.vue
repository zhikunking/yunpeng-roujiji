<template>
	<view class="review">
		<image class="review_img" src="../../static/img/no.png" mode=""></image>
		<view class="review_yes">
				审核失败，您填写的信息有误，如需继续 申请，请重新提交申请
		</view>
		<view class="review_btn1">
			重新申请
		</view>
		<view class="review_btn2">
			返回
		</view>
	</view>
</template>

<script>
</script>

<style>
	.review{
		height: 1364rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		position: relative;
	}
	.review_img{
		width: 654rpx;
		height: 410rpx;
		margin: 62rpx 48rpx 100rpx 48rpx;
	}
	.review_yes{
		width: 504rpx;
		height: 80rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
		line-height: 40rpx;
		text-align: center;
		margin: 0 auto;
	}
	.review_btn1{
		width: 690rpx;
		height: 88rpx;
		background: #3891ED;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		margin-top: 404rpx;
		margin-left: 30rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #FFFFFF;
		line-height: 88rpx;
		text-align: center;
	}
	.review_btn2{
		width: 690rpx;
		height: 88rpx;
		background: #EAEAEA;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		margin-top: 40rpx;
		margin-left: 30rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 88rpx;
		text-align: center;
	}
</style>