<template>
	<view class="search">
		<view class="search-top">
			<image class="search-top-img" src="../../static/img/search2.png" mode=""></image>
			<input class="search-top-input" type="text" placeholder="搜索商品">
			<button class="search-top-btn">搜索</button>
		</view>
		<view class="search-nav">
			<view class="search-nav-text">
				搜索历史
			</view>
			<view>
				<image class="search-nav-icon" src="../../static/img/del.png" mode=""></image>
			</view>
		</view>
		<view class="search-btn">
			<view class="search-btn-button" v-for="(item,index) in arr" :key="index">
				{{item.name}}
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				arr:[
					{name:"西瓜"},
					{name:"阳光玫瑰"},
					{name:"小香松"},
					{name:"土鸡蛋"},
					{name:"鲜牛奶"},
				],
			}
		},
		onLoad() {
	
		},
		methods: {
			
		},
			
	}
</script>

<style>
	.search{
		width: 100%;
		height: 1624rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.search-top{
		width: 690rpx;
		height: 80rpx;
		background: #FFFFFF;
		border-radius: 40rpx 40rpx 40rpx 40rpx;
		opacity: 1;
		border: 2rpx solid #3891ED;
		margin-left: 30rpx;
		margin-top: 40rpx;
		display: flex;
	}
	.search-top-img{
		width: 30rpx;
		height: 30rpx;
		margin-top: 24rpx;
		margin-left: 24rpx;
	}
	.search-top-input{
		width: 114rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #878787;
		line-height: 40rpx;
		margin-top: 20rpx;
		margin-left: 12rpx;
	}
	.search-top-btn{
		width: 160rpx;
		height: 72rpx;
		background: #3891ED;
		border-radius: 40rpx 40rpx 40rpx 40rpx;
		opacity: 1;
		margin-top: 4rpx;
		margin-right: 4rpx;
		color: #FFFFFF;
		line-height: 72rpx;
		font-family: PingFang SC-Medium;
		font-weight: Medium;
		font-size: 28rpx;
	}
	.search-nav{
		margin-top: 30rpx;
		margin-left: 30rpx;
		display: flex;
		align-items: center;
		justify-content: space-between;
	}
	.search-nav-text{
		width: 128rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 38rpx;
	}
	.search-nav-icon{
		margin-right: 32rpx;
		width: 34rpx;
		height: 36rpx;
		opacity: 1;
	}
	.search-btn{
		display: flex;
		flex-wrap: wrap;
	}
	.search-btn-button{
		width: 210rpx;
		height: 68rpx;
		background: #F4F4F4;
		border-radius: 40rpx 40rpx 40rpx 40rpx;
		opacity: 1;
		margin-left: 30rpx;
		margin-top: 30rpx;
		color: #333333;
		line-height: 68rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-size: 28rpx;
		text-align: center;
	}
</style>