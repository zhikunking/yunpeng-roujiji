<template>
	<view>
		<view class="my-tousu-list" v-for="(item,index) in list" :key="index">
			<view class="my-tousu-list-yi">
				<image class="my-tousu-list-yi-img" :src="item.url" mode=""></image>
				<view class="my-tousu-list-yi-text1">{{item.name1}}</view>
				<view class="my-tousu-list-yi-text2">{{item.name2}}</view>
			</view>
			<view class="my-tousu-list-er">
				<view class="my-tousu-list-er-text1">
					{{item.name3}}
				</view>
				<view class="my-tousu-list-er-text2">
					{{item.name4}}
				</view>
				<view class="my-tousu-list-er-text3">
					{{item.name5}}
				</view>
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
						url:'../../static/img/image.png',
						name1:'投诉人：王小明',
						name2:'三天前',
						name3:'投诉对象：山东肉集集信息科技有限责任公司',
						name4:'投诉类型：诈骗',
						name5:'投诉描述：描述内容内容内容内容内容内容内容'
					},
					{
						url:'../../static/img/image.png',
						name1:'投诉人：王小明',
						name2:'三天前',
						name3:'投诉对象：山东肉集集信息科技有限责任公司',
						name4:'投诉类型：诈骗',
						name5:'投诉描述：描述内容内容内容内容内容内容内容'
					}
				]
			}
		}
	}
</script>

<style>
	.my-tousu-list{
		height: 330rpx;
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
	.my-tousu-list-yi-img{
		width: 60rpx;
		height: 60rpx;
		margin-left: 30rpx;
	}
	.my-tousu-list-yi-text1{
		/* width: 196rpx; */
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 33rpx;
		margin-left: 20rpx;
	}
	.my-tousu-list-yi-text2{
		/* width: 74rpx; */
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
		margin-left: 282rpx;
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
	.my-tousu-list-er-text2{
		/* width: 210rpx; */
		height: 42rpx;
		font-size: 30rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 35rpx;
		margin-bottom: 20rpx;
	}
	.my-tousu-list-er-text3{
		/* width: 630rpx; */
		height: 42rpx;
		font-size: 30rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 35rpx;
	}
</style>