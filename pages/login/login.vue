<template>
	<view class="login">
		<uni-nav-bar left-icon="left"></uni-nav-bar>
		<view class="login-text">
			欢迎登录肉集集
		</view>
		<view class="login-input">
			<text class="login-input-text">+86</text>
			<image class="login-input-image" src="../../static/img/xia.png" mode=""></image>
			<text class="login-input-text2" type="text"></text>
			<input class="login-text-input" v-model="phone.val" @blur="teltest" placeholder="请输入手机号" maxlength="11"/>
		</view>
		<view class="login-password">
			<input @input="clickVerification" class="login-password-text" placeholder="请输入验证码" type="text">
			<text class="login-password-text2" @click="getVerification">获取验证码</text>
		</view>
		<view class="login-text2">
			<view @click="agree" v-if="agreeStatus == false">
				<image class="login-text2-img1" src="/static/img/yuan.png"></image>
			</view>
			<view @click="agree" v-else>
				<image class="login-text2-img1" src="../../static/img/tubiao.png"></image>
			</view>
			<text class="login-text-text1">我已阅读并同意<text class="login-text-text2">《用户协议》</text>和<text class="login-text-text2">《隐私协议》</text>未注册手机号将自动注册</text> 
		</view>
		<button class="login-login1" @click="logon">登录/注册</button>
		<view class="login-bottom" @click="pasLogin">密码登录</view>
	</view>
</template>
<script>
	export default {
		data() {
			return {
				phone: {
				        val: '15838985085'
				},
				agreeStatus:false,
			}
		},
		onLoad() {
	
		},
		methods: {
			teltest (type) {
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
			btn(){
				
			},
			logon(){
				this.type = 'type'
				const reg = /^1([38]\d|5[0-35-9]|7[3678])\d{8}$/;
				if(!this.phone.val){
					uni.showToast({
						title: '请填写手机号',
						icon:'none',
						duration: 2000
					});
					return false
				}else if (this.phone.val.length <= 10 || !reg.test(this.phone.val)) {
					uni.showToast({
						title: '手机号码错误',
						icon:'none',
						duration: 2000
					});
				    return false
				}else{
					uni.navigateTo({
						url:'/pages/login/logon'
					})
				}
			},
			pasLogin(){
				uni.navigateTo({
					url:'/pages/login/index2'
				})
			},
			getVerification(){
				if(this.phone.val == ''){
					uni.showToast({
						title: '请填写手机号',
						icon:'none',
						duration: 2000
					});
					return false
				}
			},
			clickVerification(e){
				console.log(e)
			},
			agree(){
				this.agreeStatus = !this.agreeStatus
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
		margin-right: 402rpx;
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
	.login-input-text{
		width: 58rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 38rpx;
		margin-right: 10rpx;
		margin-left: 30rpx;
	}
	.login-input-image{
		width: 40rpx;
		height: 40rpx;
	}
	.login-input-text2{
		width: 2rpx;
		opacity: 1;
		height: 60rpx;
		background-color: #CCCCCC;
		margin-left: 14rpx;
	}
	.login-text-input{
		margin-left: 30rpx;
	}
	.login-password{
		/* width: 650rpx; */
		height: 104rpx;
		background: #F3F3F3;
		border-radius: 20rpx 20rpx 20rpx 20rpx;
		opacity: 1;
		margin-top: 30rpx;
		margin-left: 50rpx;
		margin-right: 50rpx;
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
	.login-password-text2{
		width: 140rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #3891ED;
		line-height: 32rpx;
		margin-left: 258rpx;
		margin-top: 12rpx;
	}
	.login-text2{
		width: 680rpx;
		display: flex;
	}
	.login-text2-img1{
		margin-top: 46rpx;
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
		/* width: 690rpx; */
		height: 88rpx;
		background: #3891ED;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		margin-top: 160rpx;
		margin-left: 30rpx;
		margin-right: 30rpx;
		line-height: 88rpx;
		color: #FFFFFF;
		font-size: 32rpx;
		font-weight: Bold;
		font-family: PingFang SC-Bold;
	}
	.login-bottom{
		/* width: 112rpx; */
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #3891ED;
		line-height: 32rpx;
		margin-top: 30rpx;
		margin-left: 318rpx;
		margin-right: 320rpx;
		text-align: center;
	}
</style>