<template>
	<view>
		<view class="search-list-one" v-for="(item, index) in shopList" :key="index" @click="tzShoppList">
				<image :src="item.url1" class="search-list-one-img"></image>
				<view class="search-list-one-text">
					<view class="search-list-one-text-left1">
						{{item.name1}}
					</view>
					<view style="margin-top: 8rpx;" class="search-list-one-text-left2">
						{{item.name2}}
					</view>
					<view class="search-list-one-text-left2">
						{{item.name3}}
						<view class="search-list-one-text-right1-text">
							{{item.name6}}
						</view>
					</view>
					<view class="search-list-one-text-left2">
						{{item.name4}}
						<image class="search-list-one-text-right2-img" :src="item.url2"></image>
						<view class="search-list-one-text-right2-text1">
							{{item.name7}}
						</view>
					</view>
					<view class="search-list-one-text-left3">
						{{item.name5}}
						<view class="search-list-one-text-right2-text2">
							{{item.name8}}
						</view>
					</view>
				</view>
		</view>
	</view>
	
</template>

<script>
	export default {
		data() {
			return {
				shopList:[
					{
						url1:"../../static/img/root2.png",
						url2:"../../static/img/weizhi2.png",
						name1:"商品名称",
						name2:"搜索抓到的sku名称",
						name3:"母猪产品鲜品",
						name4:"中国-厂家名称",
						name5:"张三信息科技有限公司",
						name6:"￥35/千克",
						name7:"100km",
						name8:"进店",
					},
					{
						url1:"../../static/img/root2.png",
						url2:"../../static/img/weizhi2.png",
						name1:"商品名称",
						name2:"搜索抓到的sku名称",
						name3:"母猪产品鲜品",
						name4:"中国-厂家名称",
						name5:"张三信息科技有限公司",
						name6:"￥15/千克",
						name7:"100km",
						name8:"进店",
					},
					{
						url1:"../../static/img/root2.png",
						url2:"../../static/img/weizhi2.png",
						name1:"商品名称",
						name2:"搜索抓到的sku名称",
						name3:"母猪产品鲜品",
						name4:"中国-厂家名称",
						name5:"张三信息科技有限公司",
						name6:"￥15/千克",
						name7:"100km",
						name8:"进店",
					},
					{
						url1:"../../static/img/root2.png",
						url2:"../../static/img/weizhi2.png",
						name1:"商品名称",
						name2:"搜索抓到的sku名称",
						name3:"母猪产品鲜品",
						name4:"中国-厂家名称",
						name5:"张三信息科技有限公司",
						name6:"￥15/千克",
						name7:"100km",
						name8:"进店",
					}
				],
			}
		},
		onLoad() {
				
		},
		methods: {
			tzShoppList(){
				uni.navigateTo({
					url:'/pages/shopping/spot/intoShopList'
				})
			}
		},
	}
</script>

<style>
	.search-list-one{
		height: 236rpx;
		background: #FFFFFF;
		border-top: 2rpx solid #f5f5f5;
		display: flex;
	}
	.search-list-one-img{
		/* width: 196rpx; */
		height: 196rpx;
		margin-right: 20rpx;
		margin-top: 20rpx;
		margin-left: 30rpx;
	}
	.search-list-one-text{
		margin-right: 32rpx;
		margin-top: 20rpx;
		margin-bottom: 20rpx;
	}
	.search-list-one-text-left1{
		/* width: 128rpx; */
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 38rpx;
		margin-top: 2rpx;
	}
	.search-list-one-text-left2{
		width: 516rpx;
		/* width: 504rpx; */
		height: 34rpx;
		font-size: 24rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #666666;
		line-height: 28rpx;
		display: flex;
		margin-top: 4rpx;
	}
	.search-list-one-text-left3{
		width: 516rpx;
		/* width: 200rpx; */
		height: 28rpx;
		font-size: 20rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #666666;
		line-height: 24rpx;
		display: flex;
	}
	.search-list-one-text-right1-text{
		/* margin-left: 134rpx; */
		margin-left: 184rpx;
		/* width: 160rpx; */
		height: 34rpx;
		font-size: 32rpx;
		font-family: DIN-Bold, DIN;
		font-weight: bold;
		color: #C80000;
		line-height: 38rpx;
	}
	.search-list-one-text-right2-img{
		/* margin-left: 146rpx; */
		margin-left: 194rpx;
		width: 28rpx;
		height: 28rpx;
	}
	.search-list-one-text-right2-text1{
		/* width: 84rpx; */
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 32rpx;
		margin-left: 4rpx;
	}
	.search-list-one-text-right2-text2{
		/* width: 50rpx; */
		height: 28rpx;
		font-size: 20rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #666666;
		line-height: 24rpx;
		margin-left: 234rpx;
	}
</style>