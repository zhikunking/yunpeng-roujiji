<template>
	<view class="certification">
		<image class="certification_img" src="../../static/img/yyzz.png" mode=""></image>
		<view class="certification_text">
			请上传营业执照
		</view>
		<view class="certification_name">
			<view class="certification_name_text">
				企业名称：
			</view>
			<input class="certification_name_input" type="text" placeholder="山东肉集集信息科技有限公司">
		</view>
		<view class="certification_bottom">
			确认提交
		</view>
	</view>
</template>

<script>
</script>

<style>
	.certification{
		position: relative;
		height: 1254rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.certification_img{
		width: 472rpx;
		height: 300rpx;
		margin-top: 80rpx;
		margin-left: 140rpx;
	}
	.certification_text{
		text-align: center;
		margin-top: 30rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
	}
	.certification_name{
		height: 44rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		padding: 30rpx 50rpx;
		display: flex;
		align-items: center;
		margin-top: 60rpx;
	}
	.certification_name_text{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 38rpx;
	}
	.certification_name_input{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
		line-height: 33rpx;
		margin-left: 20rpx;
	}
	.certification_bottom{
		position: absolute;
		bottom: 0;
		width: 690rpx;
		height: 88rpx;
		background: #3891ED;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		margin: 0 auto;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #FFFFFF;
		line-height: 88rpx;
		text-align: center;
		margin: 16rpx 30rpx;
	}
</style>