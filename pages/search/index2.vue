<template>
	<view class="search2">
		<view class="search2-top">
			<view class="search2-top-search">
				<image class="search2-top-search-img" src="../../static/img/Search.png" mode=""></image>
				<input class="search2-top-search-input" type="text" placeholder="搜索">
			</view>
		</view>
		<view class="search2-top1" v-for="(item,index) in VIPlist" :key="index">
			<view class="search2-top1-wen">{{item.name}}</view>
			<image class="search2-top1-img" src="../../static/img/you.png" mode=""></image>
		</view>
	</view>
</template>

<script>
	export default {
	  data() {
	    return {
			VIPlist:[
				{name:'会员如何使用?'},
				{name:'商品退款流程'},
				{name:'怎么取消订单'},
				{name:'你到底想要怎么样？'},
			]
	    };
	  },
	  methods: {
	    
	  },
	};
</script>

<style>
	.search2{
		height: 1624rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.search2-top{
		width: 100%;
		height: 104rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;	
	}
	.search2-top-search{
		margin-top: 12rpx;
		margin-left: 30rpx;
		margin-right: 30rpx;
		width: 690rpx;
		height: 80rpx;
		background: #F5F5F5;
		border-radius: 40rpx 40rpx 40rpx 40rpx;
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
	.search2-top1{
		height: 44rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;	
		margin-top: 2rpx;
		display: flex;
		justify-content: space-between;
		align-items: center;
		padding: 30rpx;
	}
	.search2-top1-wen{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 45rpx;
	}
	.search2-top1-img{
		width: 48rpx;
		height: 48rpx;
	}
</style>