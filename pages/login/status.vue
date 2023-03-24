<template>
	<view class="login">
		<view class="login-status-text1">欢迎来到肉集集</view>
		<view class="login-status-text2">请选择您的身份，身份选择后可以随时切换</view>
		<view class="login-text1" @click="jinru">
			<view>
				<image class="login-text1-img1" src="../../static/img/card.png" mode=""></image>
			</view>
			<view class="login-text1-txt">
				<view class="login-text1-txt1">
					我要买货
				</view>
				<view class="login-text1-txt2">
					海量货源，认证商家，省心省力又省钱
				</view>
			</view>
			<view>
				<image class="login-text1-img2" src="../../static/img/you.png" mode=""></image>
			</view>
		</view>
		<view class="login-text2">
			<view>
				<image class="login-text2-img1" src="../../static/img/shopp.png" mode=""></image>
			</view>
			<view class="login-text2-txt">
				<view class="login-text2-txt1">
					我要卖货
				</view>
				<view class="login-text2-txt2">
					全网买家，及时到账不压款，无任何前置费用
				</view>
			</view>
			<view>
				<image class="login-text2-img2" src="../../static/img/you.png" mode=""></image>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data(){
			return{
				
			}
		},
		methods:{
			jinru(){
				uni.navigateTo({
					url:'/pages/home/home'
				})
			}
		}
	}
</script>

<style>
	.login-status{
		width: 100%;
		height: 88rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
	}
	.login-status-img{
		width: 48rpx;
		height: 48rpx;
		margin-left: 40rpx;
		margin-top: 20rpx;
	}
	.login-status-text1{
		width: 336rpx;
		height: 68rpx;
		font-size: 48rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 56rpx;
		margin-top: 80rpx;
		margin-left: 30rpx;
	}
	.login-status-text2{
		width: 532rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
		line-height: 32rpx;
		margin-left: 30rpx;
		margin-top: 12rpx;
	}
	.login-text1{
		width: 690rpx;
		height: 240rpx;
		background: #EBF5FF;
		border-radius: 30rpx 30rpx 30rpx 30rpx;
		opacity: 1;
		border: 4rpx solid #3891ED;
		margin-left: 30rpx;
		margin-top: 80rpx;
		display: flex;
	}
	.login-text1-img1{
		width: 84rpx;
		height: 84rpx;
		margin-left: 30rpx;
		margin-top: 78rpx;
	}
	.login-text1-txt{
		margin-top: 44rpx;
		margin-left: 34rpx;
	}
	.login-text1-txt1{
		width: 160rpx;
		height: 56rpx;
		font-size: 40rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #3891ED;
		line-height: 46rpx;
		margin-bottom: 8rpx;
	}
	.login-text1-txt2{
		width: 448rpx;
		height: 88rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 38rpx;
	}
	.login-text1-img2{
		width: 48rpx;
		height: 48rpx;
		margin-top: 96rpx;
		margin-left: 16rpx;
	}
	.login-text2{
		width: 690rpx;
		height: 240rpx;
		background: #FFF3F4;
		border-radius: 30rpx 30rpx 30rpx 30rpx;
		opacity: 1;
		border: 4rpx solid #EB3F4A;
		display: flex;
		margin-top: 40rpx;
		margin-left: 30rpx;
	}
	.login-text2-img1{
		width: 84rpx;
		height: 84rpx;
		margin-left: 30rpx;
		margin-top: 78rpx;
	}
	.login-text2-txt{
		margin-top: 44rpx;
		margin-left: 34rpx;
	}
	.login-text2-txt1{
		width: 160rpx;
		height: 56rpx;
		font-size: 40rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #EB3F4A;
		line-height: 46rpx;
	}
	.login-text2-txt2{
		width: 448rpx;
		height: 88rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 38rpx;
	}
	.login-text2-img2{
		width: 48rpx;
		height: 48rpx;
		margin-top: 96rpx;
		margin-left: 16rpx;
	}
</style>