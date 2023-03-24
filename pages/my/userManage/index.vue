<template>
	<view class="manage">
		<view class="set_top">
			<view class="set_top_left">
				账号管理
			</view>
			<view class="set_top_right">
				<view class="set_top_right_t1">
					153******32
				</view>
				<image class="set_top_right_img" src="../../../static/img/you.png" mode=""></image>
			</view>
		</view>
		<view class="set_top">
			<view class="set_top_left">
				修改密码
			</view>
			<image class="set_top_right_img" src="../../../static/img/you.png" mode=""></image>
		</view>
		<view class="set_bottom">
			退出登录
		</view>
	</view>
</template>

<script>
</script>

<style>
	.manage{
		height: 1254rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		position: relative;
	}
	.manage_top{
		height: 44rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		padding: 30rpx;
	}
	.manage_top_text{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 38rpx;
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
	.set_bottom{
		position: absolute;
		bottom: 0;
		margin: 0 30rpx 16rpx 30rpx;
		width: 690rpx;
		height: 88rpx;
		line-height: 88rpx;
		text-align: center;
		background: #3891ED;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #FFFFFF;
	}
</style>