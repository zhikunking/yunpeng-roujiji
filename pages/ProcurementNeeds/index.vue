<template>
	<view class="needs">
		<view class="needs-text">
			<view class="needs-text-t1">
				文字描述（非必填）
			</view>
			<view class="needs-text-t2">
				<view class="needs-text-t2-text1">
					0/50
				</view>
				<image class="needs-text-t2-img" src="../../static/img/right2.png" mode=""></image>
			</view>
		</view>
		<textarea class="needs-kuang" placeholder="你可以填写内容"></textarea>
		<view class="needs-text">
			<view class="needs-text-t1">
				上传图片（非必填）
			</view>
			<view class="needs-text-t2">
				<view class="needs-text-t2-text1">
					0/3
				</view>
				<image class="needs-text-t2-img" src="../../static/img/right2.png" mode=""></image>
			</view>
		</view>
		<view class="needs-img">
			<view class="needs-img-text1">
				+
			</view>
			<view class="needs-img-text2">
				上传
			</view>
		</view>
		<view class="needs-bottom">
			完成
		</view>
	</view>
</template>

<script>
</script>

<style>
	.needs{
		height: 1164rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		position: relative;
	}
	.needs-text{
		height: 104rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		display: flex;
		align-items: center;
		justify-content: space-between;
	}
	.needs-text-t1{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 38rpx;
		margin-left: 30rpx;
	}
	.needs-text-t2{
		margin-top: 18rpx;
		display: flex;
	}
	.needs-text-t2-text1{
		width: 66rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
		line-height: 33rpx;
	}
	.needs-text-t2-img{
		width: 40rpx;
		height: 40rpx;
		margin-top: -4rpx;
		margin-right: 30rpx;
	}
	.needs-kuang{
		width: 660rpx;
		height: 320rpx;
		border-radius: 20rpx 20rpx 20rpx 20rpx;
		opacity: 1;
		border: 2rpx solid #C1C1C1;
		margin-left: 30rpx;
		padding: 30rpx 0 0 30rpx;
	}
	.needs-img{
		margin-left: 30rpx;
		width: 160rpx;
		height: 160rpx;
		background: #FFFFFF;
		border-radius: 12rpx 12rpx 12rpx 12rpx;
		opacity: 1;
		border: 2rpx solid #999999;
		text-align: center;
		/* line-height: 160rpx; */
	}
	.needs-img-text1{
		width: 40rpx;
		height: 70rpx;
		font-size: 64rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #999999;
		line-height: 75rpx;
		margin-left: 55rpx;
		margin-top: 20rpx;
	}
	.needs-img-text2{
		height: 28rpx;
		font-size: 20rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #999999;
		line-height: 23rpx;
	}
	.needs-bottom{
		width: 690rpx;
		height: 88rpx;
		background: #3891ED;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		margin-left: 30rpx;
		position: absolute;
		bottom: 0;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #FFFFFF;
		text-align: center;
		line-height: 88rpx;
	}
</style>