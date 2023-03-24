<template>
	<view class="submit">
		<tijiao />
		<view class="submit-address">
			<view class="submit-address-left">
				要货时间
			</view>
			<view class="submit-address-right">
				<view class="submit-address-right-text">请选择要货时间</view>
				<image class="submit-address-right-img" src="../../static/img/right2.png"></image>
			</view>
		</view>
		<view class="bill-btn">
			<view class="bill-btn-text">
				配送方式
			</view>
			<view class="bill-btn-right">
				<image  class="bill-btn-right-img" src="../../static/img/yuan2.png" mode=""></image>
				<view class="bill-btn-right-text">
					自提
				</view>
			</view>
			<view class="bill-btn-right2">
				<image  class="bill-btn-right2-img" src="../../static/img/yuan1.png" mode=""></image>
				<view class="bill-btn-right2-text">
					厂家配送
				</view>
			</view>
		</view>
		<view class="submit-address2">
			<view class="submit-address2-text1">
				开具发票
			</view>
			<view class="submit-address2-text2">
				<u-switch v-model="value" @change="change"></u-switch>
			</view>
		</view>
		<view class="submit-address3">
			<view class="submit-address-left">
				订单备注
			</view>
			<view class="submit-address-right">
				<view class="submit-address-right-text1">无备注</view>
				<image class="submit-address-right-img" src="../../static/img/right2.png"></image>
			</view>
		</view>
		<kefu />
		<tijiaod/>
	</view>
</template>

<script>
	import tijiao from "@/pages/submit/indextijiao2.vue"
	import kefu from "@/pages/submit/kefu.vue"
	import tijiaod from "@/pages/submit/tijiaodingdan.vue"
	export default{
		components:{
			tijiao,
			kefu,
			tijiaod
		},
		data(){
			return{
				 value:false
				 
			}
		},
		methods:{
			change(e) {
				// console.log('change', e);
				// e.change = this.value
			},
		}
	}
</script>

<style>
	.submit{
		height: 1324rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.submit-address{
		height: 104rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		margin-top: 20rpx;
		display: flex;
		align-items: center;
		justify-content: space-between;
	}
	.submit-address-left{
		width: 128rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 38rpx;
		margin-left: 40rpx;
	}
	.submit-address-right{
		height: 90rpx;
		display: flex;
		align-items: center;
	}
	.submit-address-right-text{
		width: 196rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
		line-height: 40rpx;
	}
	.submit-address-right-text1{
		width: 84rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
		line-height: 40rpx;
	}
	.submit-address-right-img{
		width: 40rpx;
		height: 40rpx;
		margin-right: 40rpx;
	}
	.bill-btn{
		height: 104rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		border-bottom: 2rpx solid #F5F6F7;
		border-top: 2rpx solid #F5F6F7;
		display: flex;
		align-items: center;
	}
	.bill-btn-text{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 38rpx;
		margin-left: 40rpx;
	}
	.bill-btn-right{
		display: flex;
		align-items: center;
		margin-left: 196rpx;
	}
	.bill-btn-right-img{
		width: 56rpx;
		height: 56rpx;
	}
	.bill-btn-right-text{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
		margin-left: 6rpx;
		margin-top: 4rpx;
	}
	.bill-btn-right2{
		display: flex;
		align-items: center;
		margin-left: 40rpx;
	}
	.bill-btn-right2-img{
		width: 56rpx;
		height: 56rpx;
	}
	.bill-btn-right2-text{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
		margin-left: 8rpx;
		margin-top: 4rpx;
	}
	.submit-address2{
		display: flex;
		align-items: center;
		padding-left: 40rpx;
		height: 104rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		border-bottom: 2rpx solid #F5F6F7;
	}
	.submit-address2-text1{
		width: 128rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 38rpx;
	}
	.submit-address2-text2{
		margin-left: 430rpx;
	}
	.submit-address3{
		height: 104rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		display: flex;
		align-items: center;
		justify-content: space-between;
	}
</style>