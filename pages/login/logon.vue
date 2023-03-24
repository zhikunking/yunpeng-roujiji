<template>
	<view class="logon">
		<!-- <uni-nav-bar left-icon="closeempty"></uni-nav-bar> -->
		<view class="logon-text1">
			设置密码
		</view>
		<view class="logon-text2">
			166****7221尚未注册，请设置您的账号密码
		</view>
		<view class="logon-password">
			<image class="logon-password-img" src="../../static/img/suo.png" mode=""></image>
			<text class="logon-password-text">密码</text>
		</view>
		<input class="logon-password-input" type="password" placeholder="请输入8-12位数字、字母">
		<view class="logon-password-x"></view>
		<view class="logon-password2">
			<image class="logon-password2-img" src="../../static/img/suo.png" mode=""></image>
			<text class="logon-password2-text">再次输入密码</text>
		</view>
		<input class="logon-password-input" type="password" placeholder="请输入8-12位数字、字母">
		<view class="logon-password-x"></view>
		<view class="logon-text3">
			<view @click="agree" v-if="agreeStatus == false">
				<image class="logon-text3-img1" src="../../static/img/yuan.png" mode=""></image>
			</view>
			<view @click="agree" v-else>
				<image class="logon-text3-img1" src="../../static/img/tubiao.png" mode=""></image>
			</view>
			<text class="logon-text3-text1">已阅读并同意<text class="logon-text3-text2">《用户协议》</text>和<text class="logon-text3-text2">《隐私协议》</text></text> 
		</view>
		<button class="logon-bottom" @click="toNext">完成</button>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				agreeStatus:false,
			}
		},
		onLoad() {
	
		},
		methods: {
			agree(){
				this.agreeStatus =! this.agreeStatus
			},
			toNext(){
				uni.navigateTo({
					url:'/pages/login/index2'
				})
			}
		}
	}
</script>

<style>
	.logon{
		width: 100%;
		height: 1624rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.logon-text1{
		width: 176rpx;
		height: 62rpx;
		font-size: 44rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 52rpx;
		margin-left: 40rpx;
		margin-top: 60rpx;
	}
	.logon-text2{
		padding-left: 42rpx;
		margin-top: 8rpx;
		width: 480rpx;
		height: 34rpx;
		font-size: 24rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
		line-height: 28rpx;
	}
	.logon-password{
		width: 122rpx;
		height: 48rpx;
		display: flex;
		margin-top: 60rpx;
		margin-left: 42rpx;
	}
	.logon-password-img{
		width: 48rpx;
		height: 48rpx;
		margin-right: 10rpx;
	}
	.logon-password-text{
		width: 64rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 38rpx;
	}
	.logon-password-input{
		width: 320rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #999999;
		line-height: 32rpx;
		margin-top: 40rpx;
		margin-left: 44rpx;
	}
	.logon-password-x{
		width: 668rpx;
		height: 0rpx;
		opacity: 1;
		border: 1px solid #EEEEEE;
		margin-left: 44rpx;
		margin-top: 30rpx;
	}
	.logon-password2{
		width: 250rpx;
		height: 48rpx;
		display: flex;
		margin-top: 60rpx;
		margin-left: 42rpx;
	}
	.logon-password2-img{
		width: 48rpx;
		height: 48rpx;
		margin-right: 10rpx;
	}
	.logon-password2-text{
		width: 192rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 38rpx;
	}
	.logon-text3{
		display: flex;
	}
	.logon-text3-img1{
		margin-top: 162rpx;
		margin-left: 86rpx;
		width: 40rpx;
		height: 40rpx;
	}
	.logon-text3-text1{
		width: 532rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #666666;
		line-height: 40rpx;
		margin-top: 162rpx;
		margin-right: 10rpx;
	}
	.logon-text3-text2{
		color: #3891ED;
	}
	.logon-bottom{
		width: 690rpx;
		height: 88rpx;
		background: #3891ED;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		line-height: 88rpx;
		margin-top: 40rpx;
		margin-left: 30rpx;
		color: #FFFFFF;
		font-size: 32rpx;
		font-weight: Bold;
		font-family: PingFang SC-Bold;
	}
</style>