<template>
	<view class="notification">
		<view class="notification-top" v-for="(item,index) in list" :key="index">
			<view class="notification-top-yi">{{item.name1}}</view>
			<view class="notification-top2">
				<view class="notification-top-er">{{item.name2}}</view>
				<view class="notification-top-er-t1">{{item.name3}}</view>
				<view class="notification-top-er-t2"></view>
			</view>
			<view class="notification-top-san">{{item.name4}}</view>
		</view>
	</view>
</template>

<script>
	export default{
		data(){
			return{
				list:[
					{
						name1:'（报价单）鸡胸肉 冻品 50千克 / 鸡翅 冻品 50千克 /鸡胸肉 冻品 50千克',
						name2:'（询价单）',
						name3:'鸡胸肉 冻品 50千克 / 鸡翅 冻品',
						name4:'2019-03-21'
					},
					{
						name1:'（报价单）鸡胸肉 冻品 50千克 / 鸡翅 冻品 50千克 /鸡胸肉 冻品 50千克',
						name2:'（询价单）',
						name3:'鸡胸肉 冻品 50千克 / 鸡翅 冻品',
						name4:'2019-03-21'
					},
					{
						name1:'（报价单）鸡胸肉 冻品 50千克 / 鸡翅 冻品 50千克 /鸡胸肉 冻品 50千克',
						name2:'（询价单）',
						name3:'鸡胸肉 冻品 50千克 / 鸡翅 冻品',
						name4:'2019-03-21'
					},
					{
						name1:'（报价单）鸡胸肉 冻品 50千克 / 鸡翅 冻品 50千克 /鸡胸肉 冻品 50千克',
						name2:'（询价单）',
						name3:'鸡胸肉 冻品 50千克 / 鸡翅 冻品',
						name4:'2019-03-21'
					},
				]
			}
		}
	}
</script>

<style>
	.notification{
		height: 1624rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.notification-top{
		width: 690rpx;
		height: 246rpx;
		background: #FFFFFF;
		border-radius: 20rpx 20rpx 20rpx 20rpx;
		opacity: 1;
		padding-top: 20rpx;
		margin-left: 30rpx;
		margin-bottom: 20rpx;
	}
	.notification-top-yi{
		height: 88rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 38rpx;
		margin: 28rpx 40rpx 0 30rpx;
	}
	.notification-top-yi-text{
		height: 88rpx;
		font-size: 32rpx;
		color: #333333;
		line-height: 38rpx;
	}
	.notification-top2{
		display: flex;
		align-items: center;
		height: 40rpx;
	}
	.notification-top-er{
		margin: 20rpx 0 0 30rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 33rpx;
	}
	.notification-top-er-t1{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #666666;
		line-height: 33rpx;
		margin-top: 20rpx;
	}
	.notification-top-san{
		margin-top: 30rpx;
		margin-left: 30rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #666666;
		line-height: 33rpx;
	}
	.notification-top-er-t2{
		width: 20rpx;
		height: 20rpx;
		background: #DB0D0D;
		opacity: 1;
		border-radius: 50%;
		margin-left: 66rpx;
		margin-bottom: 20rpx;
	}
</style>