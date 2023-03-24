<template>
	<view class="change">
		<view class="change_phone">
			<view class="change_phone_img">
				<image class="change_phone_img1" src="../../static/img/shouji.png" mode=""></image>
				<view class="change_phone_text">
					手机号
				</view>
			</view>
			<input class="change_phone_input" type="text" placeholder="请输入手机号">
		</view>
		<view class="change_anquan">
			<view class="change_phone_img">
				<image class="change_phone_img1" src="../../static/img/anquan.png" mode=""></image>
				<view class="change_phone_text">
					验证码
				</view>
			</view>
			<view class="change_phone_inp">
				<input class="change_phone_input" type="text" placeholder="请输入验证码">
				<view class="change_phone_right">
					获取
				</view>
			</view>
		</view>
		<view class="change_anquan">
			<view class="change_phone_img">
				<image class="change_phone_img1" src="../../static/img/suo.png" mode=""></image>
				<view class="change_phone_text">
					新密码
				</view>
			</view>
			<input class="change_phone_input" type="text" placeholder="请输入新密码">
		</view>
		<view class="change_anquan">
			<view class="change_phone_img">
				<image class="change_phone_img1" src="../../static/img/suo.png" mode=""></image>
				<view class="change_phone_text">
					确认密码
				</view>
			</view>
			<input class="change_phone_input" type="text" placeholder="请输入8-12位数字、字母">
		</view>
		<view class="change_bottom">
			确认修改
		</view>
	</view>
</template>

<script>
</script>

<style>
	.change{
		height: 1324rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.change_phone{
		height: 116rpx;
		padding: 30rpx 0;
		margin: 0 30rpx;
		border-bottom: 2rpx solid #f6f6f6;
	}
	.change_phone_img{
		height: 48rpx;
		display: flex;
		align-items: center;
	}
	.change_phone_img1{
		width: 48rpx;
		height: 48rpx;
	}
	.change_phone_text{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		margin-left: 10rpx;
	}
	.change_phone_inp{
		display: flex;
		justify-content: space-between;
	}
	.change_phone_input{
		margin-top: 38rpx;
	}
	.change_anquan{
		height: 116rpx;
		padding: 30rpx 0;
		margin: 0 30rpx;
		border-bottom: 2rpx solid #f6f6f6;
	}
	.change_phone_right{
		width: 112rpx;
		height: 64rpx;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		border: 2rpx solid #3891ED;
		margin-top: 20rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #3891ED;
		line-height: 64rpx;
		text-align: center;
	}
	.change_bottom{
		margin-top: 160rpx;
		margin-left: 30rpx;
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