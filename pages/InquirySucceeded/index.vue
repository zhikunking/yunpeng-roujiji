<template>
	<view class="inquiry">
		<image class="inquiry-succee" src="../../static/img/chenggong.png" mode=""></image>
		<view class="inquiry-succee1">
			询价成功
		</view>
		<view class="inquiry-bottom">
			<view class="inquiry-bottom-btn1">
				继续询价
			</view>
			<view class="inquiry-bottom-btn2">
				查看询价单
			</view>
		</view>
	</view>
</template>

<script>
</script>

<style>
	.inquiry{
		height: 724rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.inquiry-succee{
		display: block;
		width: 240rpx;
		height: 240rpx;
		margin: 0 auto;
		margin-top: 100rpx;
	}
	.inquiry-succee1{
		height: 56rpx;
		font-size: 40rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 47rpx;
		text-align: center;
		margin-top: 40rpx;
	}
	.inquiry-bottom{
		height: 88rpx;
		display: flex;
		align-items: center;
		margin-top: 140rpx;
		margin-left: 30rpx;
		margin-right: 30rpx;
	}
	.inquiry-bottom-btn1{
		width: 330rpx;
		height: 88rpx;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		border: 2rpx solid #333333;
		text-align: center;
		line-height: 88rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
	}
	.inquiry-bottom-btn2{
		width: 330rpx;
		height: 88rpx;
		background: #3891ED;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		margin-left: 30rpx;
		text-align: center;
		line-height: 88rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #FFFFFF;
	}
</style>