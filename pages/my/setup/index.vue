<template>
	<view class="set">
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
				切换身份
			</view>
			<image class="set_top_right_img" src="../../../static/img/you.png" mode=""></image>
		</view>
		<view class="set_top">
			<view class="set_top_left">
				把肉集集推荐给好友
			</view>
			<image class="set_top_right_img" src="../../../static/img/you.png" mode=""></image>
		</view>
		<view class="set_bottom">
			<view class="set_top_left">
				关于肉集集
			</view>
			<image class="set_top_right_img" src="../../../static/img/you.png" mode=""></image>
		</view>
		<view class="set_bottom1">
			<view class="set_top_left">
				联系平台
			</view>
			<image class="set_top_right_img" src="../../../static/img/you.png" mode=""></image>
		</view>
	</view>
</template>

<script>
</script>

<style>
	.set{
		height: 1624rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
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
		height: 44rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		padding: 30rpx;
		display: flex;
		align-items: center;
		justify-content: space-between;
		margin-top: 20rpx;
	}
	.set_bottom1{
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
</style>