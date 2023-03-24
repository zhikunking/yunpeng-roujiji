<template>
	<view class="management">
		<view class="management_real">
			<view class="management_real_left">
				实名认证
			</view>
			<view class="management_real_right">
				<view class="management_real_right_text">
					未认证
				</view>
				<image class="management_real_right_img" src="../../static/img/you.png" mode=""></image>
			</view>
		</view>
		<view class="management_real">
			<view class="management_real_left">
				工商认证
			</view>
			<view class="management_real_right">
				<view class="management_real_right_text">
					未认证
				</view>
				<image class="management_real_right_img" src="../../static/img/you.png" mode=""></image>
			</view>
		</view>
	</view>
</template>

<script>
</script>

<style>
	.management{
		height: 1624rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.management_real{
		height: 44rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		padding: 28rpx 38rpx 32rpx 40rpx;
		display: flex;
		align-items: center;
		justify-content: space-between;
		border-top: 2rpx solid #F6F6F6;
	}
	.management_real_left{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 38rpx;
	}
	.management_real_right{
		display: flex;
	}
	.management_real_right_text{
		height: 40rpx;
		line-height: 45rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
	}
	.management_real_right_img{
		width: 48rpx;
		height: 48rpx;
	}
</style>