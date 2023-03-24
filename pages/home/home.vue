<template>
	<view class="home">
		<view class="home_search">
			<view class="home_search_yi" @click="tzSearch">
				<view class="home_search_yi_t1">
					<image class="home_search_yi_img" src="../../static/img/Search.png" mode=""></image>
					<view class="home_search_yi_text">
						搜索
					</view>
				</view>
			</view>
		</view>
		<view class="home-banner">
			<u-swiper :list="list5" @change="e => current = e.current" :autoplay="false">
				<view slot="indicator" class="indicator">
					<view class="indicator__dot" v-for="(item, index) in list5" :key="index"
						:class="[index === current && 'indicator__dot--active']">
					</view>
				</view>
			</u-swiper>
		</view>
		<view class="home-advertisement" @click="tzMessage">
			<view class="home-advertisement-btn">
				<view class="home-advertisement-btn-text">
					系统公告
				</view>
			</view>
			<view class="home-advertisement-text">
				系统公告，App功能上架提醒！！！
			</view>
		</view>
		<view class="home-nav">
			<view class="home-nav1" v-for="(item,index) in list2" :key="index" @click="tzShopp(index)">
				<image class="home-nav-img" :src="item.url" mode=""></image>
				<view class="home-nav-text">
					{{item.text}}
				</view>
			</view>
		</view>
		<view class="home-img" @click="tzBlacklist">
			<image class="home-img1" src="../../static/img/Group758.png" mode=""></image>
		</view>
		<view class="home-shopp">
			<view class="home-shopp-left">
				推荐商品
			</view>
			<view class="home-shopp-right" @click="tzShopping">
				<view class="home-shopp-right-text">更多</view>
				<image class="home-shopp-right-img" src="../../static/img/right2.png"></image>
			</view>
		</view>
		<ShoppList />
		<view class="home-enquiry">
			<view class="home-shopp">
				<view class="home-shopp-left">
					热门询价
				</view>
				<view class="home-shopp-right" @click="tzBuyda">
					<view class="home-shopp-right-text">更多</view>
					<image class="home-shopp-right-img" src="../../static/img/right2.png"></image>
				</view>
			</view>
			<view class="home-enquiry-btn">
				<view class="home-enquiry-btn1">
					<view class="home-enquiry-btn1-text1">
						正在询价
					</view>
					<view class="home-enquiry-btn1-text2">
						299999
					</view>
				</view>
				<view class="home-enquiry-btn1">
					<view class="home-enquiry-btn1-text1">
						当前报价
					</view>
					<view class="home-enquiry-btn2-text2">
						9999
					</view>
				</view>
			</view>
		</view>
	</view>
</template>

<script>
	import ShoppList from "@/pages/shopping/shopp-list.vue"
	export default {
		components: {
			ShoppList
		},
		data() {
			return {
				list5: [
					'https://cdn.uviewui.com/uview/swiper/swiper3.png',
					'https://cdn.uviewui.com/uview/swiper/swiper2.png',
					'https://cdn.uviewui.com/uview/swiper/swiper1.png',
				],
				current: 0,
				list1: [
					'https://cdn.uviewui.com/uview/swiper/swiper1.png',
					'https://cdn.uviewui.com/uview/swiper/swiper2.png',
					'https://cdn.uviewui.com/uview/swiper/swiper3.png',
				],
				list2: [{
						url: '../../static/img/Group596.png',
						text: '现货商场'
					},
					{
						url: '../../static/img/Group593.png',
						text: '期货商场'
					},
					{
						url: '../../static/img/Group598.png',
						text: '求购大厅'
					},
					{
						url: '../../static/img/Group599.png',
						text: '客户服务'
					}
				]
			}
		},
		methods: {
			tzShopping() {
				uni.navigateTo({
					url: '/pages/shopping/spot/index'
				})
			},
			tzSearch(){
				uni.navigateTo({
					url:'/pages/search/index'
				})
			},
			tzShopp(index){
				if(index == 0){
					uni.navigateTo({
						url:'/pages/shopping/spot/index'
					})
				}else if(index == 1){
					uni.navigateTo({
						url:'/pages/shopping/spot/index'
					})
				}else if(index == 2){
					uni.navigateTo({
						url:'/pages/buy/Buyda/index'
					})
				}else{
					uni.navigateTo({
						url:'/pages/search/index2'
					})
				}
			},
			tzMessage(){
				uni.navigateTo({
					url:'/pages/myMessage/myMessage'
				})
			},
			tzSpot(){
				uni.navigateTo({
					url:'/pages/buy/Buyda/index'
				})
			},
			tzBlacklist(){
				uni.navigateTo({
					url:'/pages/blacklist/blacklistindex'
				})
			}
		}
	}
</script>

<style>
	.indicator {
		@include flex(row);
		justify-content: center;

		&__dot {
			height: 6px;
			width: 6px;
			border-radius: 100px;
			background-color: rgba(255, 255, 255, 0.35);
			margin: 0 5px;
			transition: background-color 0.3s;

			&--active {
				background-color: #ffffff;
			}
		}
	}

	.indicator-num {
		padding: 2px 0;
		background-color: rgba(0, 0, 0, 0.35);
		border-radius: 100px;
		width: 35px;
		@include flex;
		justify-content: center;

		&__text {
			color: #FFFFFF;
			font-size: 12px;
		}
	}

	.home {
		width: 100%;
		height: 2286rpx;
		background: #F8F8F8;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.home_search{
		height: 64rpx;
		line-height: 88rpx;
		padding: 12rpx 30rpx;
		background: #3891ED;
	}	
	.home_search_yi{
		width: 690rpx;
		height: 64rpx;
		background: #FFFFFF;
		border-radius: 12rpx 12rpx 12rpx 12rpx;
		opacity: 1;
		display: flex;
		align-items: center;
		justify-content: space-evenly;
	}
	.home_search_yi_img{
		width: 36rpx;
		height: 36rpx;
	}
	.home_search_yi_t1{
		display: flex;
		align-items: center;
	}
	.home_search_yi_text{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
		line-height: 40rpx;
		margin-left: 2rpx;
	}
	.home-banner {
		margin: 20rpx 30rpx 40rpx 30rpx;
	}

	.home-advertisement {
		width: 690rpx;
		height: 80rpx;
		background: #FFFFFF;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		border: 2rpx solid #3891ED;
		margin-left: 30rpx;
		display: flex;
		align-items: center;
	}

	.home-advertisement-btn {
		width: 172rpx;
		height: 80rpx;
		background: #3891ED;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
	}

	.home-advertisement-btn-text {
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #FFFFFF;
		line-height: 39rpx;
		margin-top: 20rpx;
		margin-left: 28rpx;
	}

	.home-advertisement-text {
		width: 460rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 39rpx;
		margin-left: 20rpx;
	}

	.home-nav {
		height: 146rpx;
		display: flex;
		align-items: center;
		justify-content: space-around;
		margin-top: 40rpx;
	}

	.home-nav-img {
		width: 88rpx;
		height: 88rpx;
	}

	.home-nav1 {
		text-align: center;
	}

	.home-nav-text {
		width: 112rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #000000;
		line-height: 33rpx;
		margin-top: 18rpx;
	}

	.home-img {
		width: 690rpx;
		height: 180rpx;
		border-radius: 12rpx 12rpx 12rpx 12rpx;
		opacity: 1;
		margin: 40rpx 30rpx 12rpx 30rpx;
	}

	.home-img1 {
		width: 690rpx;
		height: 180rpx;
	}

	.home-shopp {
		width: 100%;
		height: 90rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		display: flex;
		align-items: center;
		justify-content: space-between;
	}

	.home-shopp-left {
		width: 128rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 38rpx;
		margin-left: 30rpx;
	}

	.home-shopp-right {
		width: 120rpx;
		height: 90rpx;
		display: flex;
		align-items: center;
	}

	.home-shopp-right-text {
		width: 56rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
		line-height: 40rpx;
	}

	.home-shopp-right-img {
		width: 40rpx;
		height: 40rpx;
	}

	.home-shoppList {
		height: 236rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
	}

	.home-enquiry {
		width: 100%;
		height: 334rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
	}

	.home-enquiry-left {
		margin-top: 30rpx;
		margin-left: 30rpx;
		width: 128rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 38rpx;
	}

	.home-enquiry-btn {
		margin: 30rpx;
		height: 200rpx;
		display: flex;
		justify-content: space-between;
	}

	.home-enquiry-btn1 {
		width: 330rpx;
		height: 200rpx;
		background: #F5F5F5;
		border-radius: 32rpx 32rpx 32rpx 32rpx;
		opacity: 1;
		border: 2rpx solid #999999;
	}

	.home-enquiry-btn1-text1 {
		width: 330rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 33rpx;
		text-align: center;
		margin-top: 42rpx;
	}

	.home-enquiry-btn1-text2 {
		width: 330rpx;
		height: 64rpx;
		font-size: 60rpx;
		font-family: DIN-Bold, DIN;
		font-weight: bold;
		color: #333333;
		line-height: 70rpx;
		text-align: center;
	}

	.home-enquiry-btn {
		margin: 30rpx;
		height: 200rpx;
		display: flex;
		justify-content: space-between;
	}

	.home-enquiry-btn2-text2 {
		width: 330rpx;
		height: 64rpx;
		font-size: 60rpx;
		font-family: DIN-Bold, DIN;
		font-weight: bold;
		color: #3891ED;
		line-height: 70rpx;
		text-align: center;
	}
</style>
