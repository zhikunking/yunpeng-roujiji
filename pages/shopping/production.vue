<template>
	<view class="production">
		<view class="production-top">
			<image class="production-top-img" src="../../static/img/Search.png" mode=""></image>
			<input class="production-top-input" type="text" placeholder="请搜索">
		</view>
		<view class="production-select">已选（0/6）</view>
		<view class="production-quantity">
			<view class="production-quantity-one" v-for="(item,index) in list" :key="index">
				{{item}}
				<image class="production-quantity-img" src="../../static/img/x.png" mode=""></image>
			</view>
		</view>
		<view class="production-search">热门搜索</view>
		<view class="production-search-select">
			<view class="production-search-select-one" v-for="(item,index) in list1" :key="index">{{item}}</view>
		</view>
	</view>
</template>

<script>
	export default {
	  data() {
	    return {
			list:['中国','韩国','美国','俄罗斯'],
			list1: ['不限','中国','巴西','西班牙','德国','美国','荷兰','丹麦','印尼','日本','韩国','法国'],
	    };
	  },
	  methods: {
	    
	  },
	};
</script>

<style>
	.production{
		width: 100%;
		height: 1398rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.production-top{
		width: 690rpx;
		height: 80rpx;
		background: #F5F5F5;
		border-radius: 40rpx 40rpx 40rpx 40rpx;
		opacity: 1;
		margin-top: 10rpx;
		margin-left: 30rpx;
		display: flex;
		align-items: center;
	}
	.production-top-img{
		width: 37rpx;
		height: 36rpx;
		margin-left: 284rpx;
	}
	.production-top-input{
		margin-left: 8rpx;
	}
	.production-select{
		margin-top: 30rpx;
		margin-left: 40rpx;
		width: 184rpx;
		height: 58rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 58rpx;
	}
	.production-quantity{
		display: flex;
		margin-top: 42rpx;
		margin-left: 40rpx;
	}
	.production-quantity-one{
		position: relative;
		width: 161rpx;
		height: 72rpx;
		border-radius: 12rpx 12rpx 12rpx 12rpx;
		opacity: 1;
		border: 2rpx solid #999999;
		line-height: 72rpx;
		text-align: center;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #666666;
		margin-right: 18rpx;
	}
	.production-quantity-img{
		position: absolute;
		right: -14%;
		top: -27%;
		width: 44rpx;
		height: 44rpx;
	}
	.production-search{
		margin-top: 60rpx;
		margin-left: 40rpx;
		width: 128rpx;
		height: 58rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 58rpx;
	}
	.production-search-select{
		width: 100%;
		display: flex;
		flex-wrap: wrap;
		margin-left: 40rpx;
	}
	.production-search-select-one{
		width: 161rpx;
		height: 72rpx;
		border-radius: 12rpx 12rpx 12rpx 12rpx;
		opacity: 1;
		border: 2rpx solid #999999;
		line-height: 72rpx;
		text-align: center;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #666666;
		margin-right: 12rpx;
		margin-top: 20rpx;
	}
</style>