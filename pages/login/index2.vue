<template>
	<view class="login">
		<!-- <uni-nav-bar left-icon="left"></uni-nav-bar> -->
		<view class="login-text">
			欢迎登录肉集集
		</view>
		<view class="login-input">
			<input class="login-text-input" v-model="phone.val" @blur="teltest" placeholder="请输入手机号" maxlength="11"/>
		</view>
		<view class="login-password">
			<input class="login-password-text" placeholder="请输入密码" type="password">
		</view>
		<view class="login-text2">
			<view @click="agree" v-if="agreeStatus == false">
				<image class="login-text2-img1" src="../../static/img/yuan.png" mode=""></image>
			</view>
			<view @click="agree" v-else>
				<image class="login-text2-img1" src="../../static/img/tubiao.png" mode=""></image>
			</view>
			<text class="login-text-text1">我已阅读并同意<text class="login-text-text2">《用户协议》</text>和<text class="login-text-text2">《隐私协议》</text></text> 
		</view>
		<view class="bottom">
			<button class="login-login1" @click="paslogin">登录</button>
			<view class="login-bottom" @click="login">短信验证码登录</view>
			<view class="login-bottom2" @click="noLogin">忘记密码</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				phone: {
				        val: ''
				},
				agreeStatus:false
			}
		},
		onLoad() {
	
		},
		methods: {
			paslogin(){
				uni.navigateTo({
					url:'/pages/login/status'
				})
			},
			teltest () {
			    const reg = /^1([38]\d|5[0-35-9]|7[3678])\d{8}$/;
			    if(!this.phone.val){
			    	
			    	return false
			    }else if (this.phone.val.length <= 10 || !reg.test(this.phone.val)) {
			    	uni.showToast({
			    		title: '手机号码错误',
			    		icon:'none',
			    		duration: 2000
			    	});
			        return false
			    }
			},
			login(){
				uni.navigateTo({
					url:'/pages/login/index'
				})
			},
			noLogin(){
				uni.navigateTo({
					url:'/pages/login/noPassword'
				})
			},
			agree(){
				this.agreeStatus =! this.agreeStatus
			}
		}
	}
</script>

<style>
	.login{
		/* width: 750rpx; */
		height: 1624rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.login-text{
		margin-top: 40rpx;
		margin-left: 40rpx;
		color: #333333;
		font-size: 44rpx;
		font-family: PingFang SC-Bold;
		font-weight: Bold;
	}
	.login-input{
		/* width: 650rpx; */
		height: 104rpx;
		background: #F3F3F3;
		border-radius: 20rpx 20rpx 20rpx 20rpx;
		opacity: 1;
		margin-top: 94rpx;
		margin-left: 50rpx;
		margin-right: 50rpx;
		display: flex;
		align-items: center;
	}
	.login-text-input{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #999999;
		line-height: 32rpx;
		/* margin-top: 40rpx; */
		margin-left: 30rpx;
	}
	.login-password{
		/* width: 650rpx; */
		height: 104rpx;
		background: #F3F3F3;
		border-radius: 20rpx 20rpx 20rpx 20rpx;
		opacity: 1;
		margin-top: 30rpx;
		margin-right: 50rpx;
		margin-left: 50rpx;
		display: flex;
		align-items: center;
	}
	.login-password-text{
		width: 192rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #999999;
		line-height: 38rpx;
		margin-left: 30rpx;
	}
	.login-text2{
		display: flex;
	}
	.login-text2-img1{
		margin-top: 42rpx;
		margin-left: 74rpx;
		width: 40rpx;
		height: 40rpx;
	}
	.login-text-text1{
		width: 560rpx;
		height: 80rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #666666;
		line-height: 32rpx;
		margin-top: 46rpx;
		margin-left: 8rpx;
	}
	.login-text-text2{
		color: #3891ED;
	}
	.login-login1{
		width: 690rpx;
		height: 88rpx;
		background: #3891ED;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		margin-top: 160rpx;
		margin-left: 30rpx;
		line-height: 88rpx;
		color: #FFFFFF;
		font-size: 32rpx;
		font-weight: Bold;
		font-family: PingFang SC-Bold;
	}
	.login-bottom{
		width: 196rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #3891ED;
		line-height: 32rpx;
		margin-top: 30rpx;
		margin-left: 276rpx;
	}
	.login-bottom2{
		width: 112rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 32rpx;
		margin-top: 20rpx;
		margin-left: 318rpx;
	}
	.bottom{
		width: 100%;
	}
</style>