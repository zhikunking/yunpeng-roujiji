<template>
	<view class="logon">
		<view class="logon-text1">
			绑定新手机号
		</view>
		<view class="logon-password">
			<image class="logon-password-img" src="../../static/img/shouji.png" mode=""></image>
			<text class="logon-password-text">手机号</text>
		</view>
		<input class="logon-password-input" type="text" placeholder="请输入手机号"  v-model="phone.val" @blur="teltest()" maxlength="11">
		<view class="logon-password-x"></view>
		<view class="logon-password2">
			<image class="logon-password2-img" src="../../static/img/anquan.png" mode=""></image>
			<text class="logon-password2-text">验证码</text>
		</view>
		<view class="logon-password3">
			<input class="logon-password-input" type="text" placeholder="请输入验证码">
			<view class="logon-button" @click="getVerification">
				获取
			</view>
		</view>
		<view class="logon-password-x"></view>
		<button class="logon-bottom" @click="toNext">下一步</button>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				phone: {
				        val: ''
				},
			}
		},
		onLoad() {
	
		},
		methods: {
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
			getVerification(){
				if(!this.phone.val){
					uni.showToast({
						title: '请填写手机号',
						icon:'none',
						duration: 2000
					});
					return false
				}
			},
			toNext(){
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
						url:'/pages/login/index2'
					})
				}
				console.log(1)
			}
		}
	}
</script>

<style>
	.logon{
		/* width: 750rpx; */
		height: 1624rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.logon-text1{
		/* width: 176rpx; */
		height: 62rpx;
		font-size: 44rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 52rpx;
		margin-left: 40rpx;
		margin-top: 60rpx;
	}
	.logon-password{
		/* width: 154rpx; */
		height: 48rpx;
		display: flex;
		margin-top: 76rpx;
		margin-left: 40rpx;
	}
	.logon-password-img{
		width: 48rpx;
		height: 48rpx;
		margin-right: 10rpx;
	}
	.logon-password-text{
		width: 96rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 38rpx;
	}
	.logon-password-input{
		/* width: 320rpx; */
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
		/* width: 668rpx; */
		height: 0rpx;
		opacity: 1;
		border: 1px solid #EEEEEE;
		margin-left: 44rpx;
		margin-top: 30rpx;
	}
	.logon-password2{
		/* width: 250rpx; */
		height: 48rpx;
		display: flex;
		margin-top: 60rpx;
		margin-left: 40rpx;
	}
	.logon-password2-img{
		width: 48rpx;
		height: 48rpx;
		margin-right: 10rpx;
	}
	.logon-password3{
		display: flex;
	}
	.logon-button{
		width: 112rpx;
		height: 64rpx;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		border: 2rpx solid #3891ED;
		margin-left: 338rpx;
		margin-top: 20rpx;
		margin-right: 40rpx;
		line-height: 64rpx;
		text-align: center;
		font-size: 28rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #3891ED;
		line-height: 64rpx;
	}
	.logon-bottom{
		width: 690rpx;
		height: 88rpx;
		background: #3891ED;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		color: #FFFFFF;
		font-size: 32rpx;
		font-weight: Bold;
		font-family: PingFang SC-Bold;
		margin-top: 396rpx;
	}
</style>