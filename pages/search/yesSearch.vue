<template>
	<view class="search">
		<view class="search-top">
			<image class="search-top-img" src="../../static/img/search2.png" mode=""></image>
			<input class="search-top-input" type="text" placeholder="搜索商品">
			<image class="search-top-img2" src="../../static/img/x.png" mode=""></image>
			<button class="search-top-btn">搜索</button>
		</view>
			<ShoppList />
			<!-- <myTousu /> -->
	</view>
</template>
<script>
	import ShoppList from "@/pages/shopping/shopp-list.vue"
	import myTousu from "@/pages/tousu/fztousu.vue"
	export default {
		components:{
			ShoppList,
			myTousu
		},
		data() {
			return {
				
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
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		padding-top: 20rpx;
	}
	.search-top{
		width: 690rpx;
		height: 80rpx;
		background: #FFFFFF;
		border-radius: 40rpx 40rpx 40rpx 40rpx;
		opacity: 1;
		border: 2rpx solid #3891ED;
		margin: 0 30rpx 20rpx 30rpx;
		display: flex;
	}
	.search-top-img{
		width: 30rpx;
		height: 30rpx;
		margin-top: 24rpx;
		margin-left: 24rpx;
	}
	.search-top-img2{
		width: 44rpx;
		height: 44rpx;
		/* margin-right: 87px; */
		margin-left: 300rpx;
		margin-top: 18rpx
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
		border-radius: 40rpx;
		opacity: 1;
		margin-top: 4rpx;
		margin-right: 4rpx;
		color: #FFFFFF;
		line-height: 72rpx;
		font-family: PingFang SC-Medium;
		font-weight: Medium;
		font-size: 28rpx;
	}
</style>