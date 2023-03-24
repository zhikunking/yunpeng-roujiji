<template>
	<view class="bill">
		<view class="bill-btn">
			<view class="bill-btn-text">
				发票详情
			</view>
			<view class="bill-btn-right">
				<image  class="bill-btn-right-img" src="../../static/img/yuan2.png" mode=""></image>
				<view class="bill-btn-right-text">
					企业
				</view>
			</view>
			<view class="bill-btn-right2">
				<image  class="bill-btn-right2-img" src="../../static/img/yuan1.png" mode=""></image>
				<view class="bill-btn-right2-text">
					个人/非企业
				</view>
			</view>
		</view>
		<view class="bill-btn2" v-for="(item,index) in list" :key="index">
			<view class="bill-btn-text">
				{{item.text1}}
			</view>
			<input class="bill-btn-text2" type="text" :placeholder="item.text2">
		</view>
		<view class="bill-btn3">
			保存
		</view>
	</view>
</template>

<script>
	export default{
		data(){
			return{
				list:[
					{
						text1:'发票抬头',
						text2:'请输入'
					},
					{
						text1:'发票抬头',
						text2:'请输入'
					},
					{
						text1:'税号',
						text2:'请输入'
					},
					{
						text1:'企业地址',
						text2:'选填'
					},
					{
						text1:'企业电话',
						text2:'选填'
					},
					{
						text1:'开户银行',
						text2:'选填'
					},
					{
						text1:'银行账号',
						text2:'选填'
					},
				]
			}
		}
	}
</script>

<style>
	.bill{
		height: 1524rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.bill-btn{
		height: 104rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
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
		margin-left: 30rpx;
	}
	.bill-btn-right{
		display: flex;
		align-items: center;
		margin-left: 186rpx;
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
	.bill-btn2{
		height: 104rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		border-top: 2rpx solid #F5F6F7;
		display: flex;
		align-items: center;
		justify-content: space-between;
	}
	.bill-btn-text2{
		width: 84rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
		line-height: 33rpx;
		margin-right: 40rpx;
		text-align: right;
	}
	.bill-btn3{
		width: 690rpx;
		height: 88rpx;
		background: #3891ED;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #FFFFFF;
		text-align: center;
		margin-top: 510rpx;
		margin-left: 30rpx;
		line-height: 88rpx;
	}
</style>