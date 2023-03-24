<template>
	<view class="enquiryShopp">
		<view class="my-tousu-list" v-for="(item,index) in list" :key="index">
			<view class="my-tousu-list-yi">
				<view class="my-tousu-list-yi-text1">{{item.name1}}</view>
				<image class="my-tousu-list-yi-img" :src="item.url1" mode=""></image>
				<!-- <image class="my-tousu-list-yi-img" :src="item.url2" mode=""></image> -->
			</view>
			<view class="my-tousu-list-er">
				<view class="my-tousu-list-er-text1">
					{{item.name2}}
				</view>
			</view>
		</view>
		<view class="enquiryShopp-bottom">
			<view class="enquiryShopp-bottom-btn">
				确认
			</view>
		</view>
	</view>
</template>

<script>
	export default{
		data(){
			return{
				list:[
					{
						url1:'../../static/img/yuan1.png',
						url2:'../../static/img/yuan2.png',
						name1:'询价单1',
						name2:'鸡胸肉 冻品 50千克 / 鸡翅 冻品 50千克 /鸡胸肉 冻品 50千克 / 鸡翅 冻品 50千克 /鸡胸肉 冻品 50千克 / 鸡翅 冻品 50千克 /'
					},
					{
						url1:'../../static/img/yuan1.png',
						url2:'../../static/img/yuan2.png',
						name1:'询价单1',
						name2:'鸡胸肉 冻品 50千克 / 鸡翅 冻品 50千克 /鸡胸肉 冻品 50千克 / 鸡翅 冻品 50千克 /鸡胸肉 冻品 50千克 / 鸡翅 冻品 50千克 /'
					},
					{
						url1:'../../static/img/yuan1.png',
						url2:'../../static/img/yuan2.png',
						name1:'询价单1',
						name2:'鸡胸肉 冻品 50千克 / 鸡翅 冻品 50千克 /鸡胸肉 冻品 50千克 / 鸡翅 冻品 50千克 /鸡胸肉 冻品 50千克 / 鸡翅 冻品 50千克 /'
					}
				]
			}
		}
	}
</script>

<style>
	.enquiryShopp{
		height: 1224rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		position: relative;
	}
	.my-tousu-list{
		height: 276rpx;
		background: #FFFFFF;
		border-radius: 20rpx 20rpx 20rpx 20rpx;
		opacity: 1;
		padding-top: 20rpx;
		margin: 0 30rpx 20rpx 30rpx;
	}
	.my-tousu-list-yi{
		height: 100rpx;
		border-bottom: 2rpx solid #f9f9f9;
		display: flex;
		align-items: center;
	}
	.my-tousu-list-yi-text1{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 38rpx;
		margin-left: 30rpx;
	}
	.my-tousu-list-er{
		margin: 30rpx 30rpx 34rpx 30rpx;
	}
	.my-tousu-list-er-text1{
		/* width: 600rpx; */
		height: 42rpx;
		font-size: 30rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 35rpx;
		margin-bottom: 20rpx;
	}
	.my-tousu-list-yi-img{
		width: 56rpx;
		height: 56rpx;
		margin-left: 454rpx;
	}
	.enquiryShopp-bottom{
		position: absolute;
		width: 100%;
		bottom: 0;
		height: 120rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
	}
	.enquiryShopp-bottom-btn{
		width: 690rpx;
		height: 88rpx;
		line-height: 88rpx;
		text-align: center;
		background: #3891ED;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		margin-top: 16rpx;
		margin-left: 30rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #FFFFFF;
	}
</style>