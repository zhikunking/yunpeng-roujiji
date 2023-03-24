<template>
	<view class="news">
		<view class="news_top">
			<view class="search2-top-search">
				<image class="search2-top-search-img" src="../../static/img/Search.png" mode=""></image>
				<input class="search2-top-search-input" type="text" placeholder="搜索">
			</view>
			<view class="news_top_yi">
				<view class="news_top_yi_img1">
					<image class="news_top_yi_img1_t1" src="../../static/img/shuicon2.png" mode=""></image>
					<view class="news_top_yi_img1_t2">
						询报价通知
					</view>
				</view>
				<view class="news_top_yi_img1">
					<image class="news_top_yi_img1_t1" src="../../static/img/shuicon.png" mode=""></image>
					<view class="news_top_yi_img1_t2">
						消息
					</view>
				</view>
			</view>
		</view>
		<view class="news_bottom" v-for="(item,index) in list" :key="index">
			<image class="news_bottom-img" :src="item.url" mode=""></image>
			<view class="news_bottom-text">
				<view class="news_bottom-text-t1">
					{{item.title}}
				</view>
				<view class="news_bottom-text-t2">
					{{item.conten}}
				</view>
			</view>
			<view class="news_bottom-text2">
				{{item.rightText}}
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
						url:'../../static/img/tupian.png',
						title:'老王杂货店',
						conten:'你好，你好，什么时候发货',
						rightText:'昨天'
					},
					{
						url:'../../static/img/tupian.png',
						title:'老王杂货店',
						conten:'你好，你好，什么时候发货',
						rightText:'昨天'
					},
					{
						url:'../../static/img/tupian.png',
						title:'老王杂货店',
						conten:'你好，你好，什么时候发货',
						rightText:'昨天'
					},
				]
			}
		}
	}
</script>

<style>
	.news{
		height: 1624rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.news_top{
		height: 304rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		margin-bottom: 20rpx;
	}
	.search2-top-search{
		margin-top: 12rpx;
		margin-left: 30rpx;
		margin-right: 30rpx;
		width: 690rpx;
		height: 80rpx;
		background: #F5F5F5;
		border-radius: 12rpx 12rpx 12rpx 12rpx;
		opacity: 1;
		display: flex;
		align-items: center;
	}
	.search2-top-search-img{
		margin-left: 292rpx;
		width: 37rpx;
		height: 36rpx;
	}
	.search2-top-search-input{
		margin-left: 8rpx;
	}
	.news_top_yi{
		display: flex;
		height: 194rpx;
		margin-top: 30rpx;
	}
	.news_top_yi_img1{
		text-align: center;
		width: 50%;
	}
	.news_top_yi_img1_t1{
		width: 92rpx;
		height: 92rpx;
	}
	.news_top_yi_img1_t2{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
		margin-top: 20rpx;
	}
	.news_bottom{
		height: 84rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		padding: 38rpx 32rpx 34rpx 32rpx;
		display: flex;
		align-items: center;
		border-bottom: 2rpx solid #F8F8F8;
	}
	..news_bottom:last-child{
		border: none;
	}
	.news_bottom-img{
		width: 84rpx;
		height: 84rpx;
	}
	.news_bottom-text{
		margin-left: 26rpx;
	}
	.news_bottom-text-t1{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 38rpx;
	}
	.news_bottom-text-t2{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
		line-height: 33rpx;
		margin-top: 10rpx;
	}
	.news_bottom-text2{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
		line-height: 33rpx;
		margin-left: 184rpx;
		margin-bottom: 40rpx;
	}
</style>