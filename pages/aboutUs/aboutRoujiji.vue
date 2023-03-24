<template>
	<view class="about">
		<image class="about_logo" src="../../static/img/logo.png" mode=""></image>
		<view class="about_text1">
			肉集集
		</view>
		<view class="about_text2">
			检查版本
		</view>
		<view class="set_top">
			<view class="set_top_left">
				关于我们
			</view>
			<image class="set_top_right_img" src="../../static/img/you.png" mode=""></image>
		</view>
		<view class="set_top">
			<view class="set_top_left">
				服务协议
			</view>
			<image class="set_top_right_img" src="../../static/img/you.png" mode=""></image>
		</view>
		<view class="set_top">
			<view class="set_top_left">
				隐私政策
			</view>
			<image class="set_top_right_img" src="../../static/img/you.png" mode=""></image>
		</view>
		<view class="about_bottom">
			肉集集信息科技有限公司版权所有
		</view>
	</view>
</template>

<script>
</script>

<style>
	.about{
		height: 1624rpx;
		position: relative;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.about_logo{
		width: 200rpx;
		height: 200rpx;
		margin-top: 80rpx;
		margin-left: 276rpx;
	}
	.about_text1{
		text-align: center;
		height: 50rpx;
		font-size: 36rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 42rpx;
		margin-top: 30rpx;
	}
	.about_text2{
		text-align: center;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #3891ED;
		line-height: 33rpx;
		margin-top: 14rpx;
		margin-bottom: 100rpx;
	}
	.set_top{
		height: 44rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		padding: 30rpx;
		display: flex;
		align-items: center;
		justify-content: space-between;
		border-top: 2rpx solid #f6f6f6;
	}
	.set_top_left{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
	}
	.set_top_right{
		height: 44rpx;
		display: flex;
		align-items: center;
	}
	.set_top_right_t1{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
	}
	.set_top_right_img{
		width: 48rpx;
		height: 48rpx;
	}
	.about_bottom{
		position: absolute;
		bottom: 0;
		margin-bottom: 46rpx;
		margin-left: 166rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
	}
</style>