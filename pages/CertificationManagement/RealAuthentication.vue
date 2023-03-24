<template>
	<view class="authentication">
		<view class="authentication_top">
			<view class="authentication_top_text">
				请输入本人身份信息
			</view>
			<image class="authentication_top_img" src="../../static/img/xiangce.png" mode=""></image>
		</view>
		<view class="authentication_name">
			<view class="authentication_name_text">
				姓名：
			</view>
			<input style="margin-left:94rpx" class="authentication_name_input" type="text" placeholder="请输入真实姓名">
		</view>
		<view class="authentication_name">
			<view class="authentication_name_text">
				身份证号码：
			</view>
			<input class="authentication_name_input" type="text" placeholder="请输入身份证号码">
		</view>
		<view class="authentication_text">
			<view class="authentication_text_t1">
				温馨提示
			</view>
			<view class="authentication_text_t2">
				公民身份信息系法律责任承担主体，如您将个人信息提供给他人使用，您需要承担造成的一切法律责任，请您务必确保您是账号的使用主体。
			</view>
		</view>
	</view>
</template>

<script>
	export default{
		data(){
			return{
				
			}
		}
	}
</script>

<style>
	.authentication{
		height: 1624rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.authentication_top{
		height: 44rpx;
		padding: 30rpx;
		display: flex;
		align-items: center;
		justify-content: space-between;
	}
	.authentication_top_text{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 38rpx;
	}
	.authentication_top_img{
		width: 56rpx;
		height: 56rpx;
	}
	.authentication_name{
		height: 44rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		padding: 30rpx;
		display: flex;
		align-items: center;
		border-bottom: 2rpx solid #f6f6f6;
	}
	.authentication_name_text{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 38rpx;
	}
	.authentication_name_input{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
		line-height: 33rpx;
	}
	.authentication_text{
		width: 690rpx;
		height: 234rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #C80000;
		line-height: 33rpx;
		padding: 40rpx 30rpx;
	}
	.authentication_text_t1{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #C80000;
	}
	.authentication_text_t2{
		height: 234rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #C80000;
		line-height: 40rpx;
		text-indent: 2em;
	}
</style>