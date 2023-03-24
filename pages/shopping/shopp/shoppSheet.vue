<template>
	<view class="shopp">
		<uni-nav-bar left-icon="left" right-icon="redo" @clickRight="redo" @clickLeft="fx"></uni-nav-bar>
		<view class="shopp-top">
			  	<view class="shopp-hz">
					<view>
						<view class="shopp-top-left">
							扯的店铺，这是一家神奇的店铺
						</view>
						<view class="shopp-top-left-bottom">
							<image class="shopp-top-left-img" src="../../../static/img/qiye.png" mode=""></image>
							<image class="shopp-top-left-img" src="../../../static/img/geren.png" mode=""></image>
							<image class="shopp-top-left-img2" src="../../../static/img/changjia.png" mode=""></image>
						</view>
						
					</view>
					<image class="shopp-top-right-img" src="../../../static/img/zhaopai.png" mode=""></image>
				</view>
				<view class="shopp-top2">
					<u-line></u-line>
				</view>
			  	<view class="shopp-hz">
					<view class="shopp-hz-left">
						<view class="shopp-hz-left-text1">
							近30天报价							
						</view>
						<view class="shopp-hz-left-text2">
							0
						</view>
					</view>
					<view class="shopp-hz-right">
						<view class="shopp-hz-right-text1">
							累计成交
						</view>
						<view class="shopp-hz-right-text2">
							0
						</view>
					</view>
				</view>
		</view>
		<view class="shopp-nav">
			<view class="shopp-nav1">
				<uni-segmented-control :current="current" :values="list1" @clickItem="onClickItem" styleType="text"></uni-segmented-control>
			</view>
			<view v-show="current === 0">
				<view class="shopp-information">
					<view class="shopp-information-product1">主营产品</view>
					<view class="shopp-information-product2">产品名称、产品名称、产品名称、产品名称</view>
					<view class="shopp-information-product3">公司介绍</view>
					<view class="shopp-information-product4">公司介绍公司介绍公司介绍公司介绍公司介绍公司介绍公司介绍公司介绍公司介绍公司介绍公司介绍公司介绍公司介绍公司介绍公司介绍公司介绍</view>
					<view class="shopp-information-product5">展开全部</view>
					<view class="shopp-information-product6">店铺起售量</view>
					<view class="shopp-information-product7">500公斤</view>
					<view class="shopp-information-product8">营业执照</view>
				</view>
				<view class="shopp-contact">
					<view class="shopp-contact-text1">联系信息</view>
					<view class="shopp-contact-text2">
						<view class="shopp-contact-text2-phone">张经理 18828888210</view>
						<image class="shopp-contact-text2-img" src="../../../static/img/phone.png" mode=""></image>
					</view>
				</view>
			</view>
				
					  <view class="shopp-nav-list" v-show="current === 1">
							<view class="shopp-nav-list-shop" v-for="(item,index) in list" :key="index">
								<image class="shopp-nav-list-img" :src="item.url" mode=""></image>
								<view class="shopp-nav-list-text1">
									{{item.name1}}
								</view>
								<view class="shopp-nav-list-text2">
									{{item.name2}}
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
				current:0,
				list1:['公司信息','供应商品'],
				list:[
					{
						url:'../../../static/img/root2.png',
						name1:'商品名称商品名称商品名称',
						name2:'￥100.00'
					},
					{
						url:'../../../static/img/root2.png',
						name1:'商品名称商品名称商品名称',
						name2:'￥100.00'
					},
					{
						url:'../../../static/img/root2.png',
						name1:'商品名称商品名称商品名称',
						name2:'￥100.00'
					},
					{
						url:'../../../static/img/root2.png',
						name1:'商品名称商品名称商品名称',
						name2:'￥100.00'
					}
				]
			}
		},
		onLoad() {
	
		},
		methods: {
			qhclick(e){
				e.index = this.active
			},
			onClickItem(e) {
			      if (this.current != e.currentIndex) {
			        this.current = e.currentIndex;
			      }
			    },
				redo(){
					uni.share({
						provider:'weixin',
					})
				}
		}
	}
</script>

<style>
	.shopp-nav1{
		width: 100%;
		height: 88rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
	}
	.shopp-top2{
		padding: 0 30rpx;
		margin-top: 36rpx;
		margin-bottom: 20rpx;
	}
	.shopp-top{
		width: 100%;
		height: 314rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
	}
	.shopp{
		width: 100%;
		height: 1774rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.shopp-hz{
		display: flex;
		margin-left: 30rpx;
	}
	.shopp-top-left{
		width: 448rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 38rpx;
		margin-top: 30rpx;
		margin-bottom: 14rpx;
	}
	.shopp-top-left-img{
		width: 92rpx;
		height: 50rpx;
		margin-right: 20rpx;
	}
	.shopp-top-left-img2{
		width: 144rpx;
		height: 50rpx;
	}
	.shopp-top-right-img{
		margin-left: 118rpx;
		width: 124rpx;
		height: 124rpx;
		margin-top: 30rpx;
	}
	.shopp-hz-left-text1{
		width: 146rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 32rpx;
	}
	.shopp-hz-left-text2{
		width: 146rpx;
		height: 56rpx;
		font-size: 40rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 46rpx;
		text-align: center;
	}
	.shopp-hz-right{
		margin-left: 114rpx;
	}
	.shopp-hz-right-text1{
		width: 112rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
	}
	.shopp-hz-right-text2{
		width: 112rpx;
		height: 56rpx;
		font-size: 40rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 47rpx;
		text-align: center;
	}
	.shopp-top-left-bottom{
		display: flex;
	}
	.shopp-nav{
		margin-top: 20rpx;
	}
	.shopp-nav-list{
		width: 100%;
		height: 976rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		display: flex;
		flex-wrap: wrap;
		padding-left: 30rpx;
		padding-top: 30rpx;
	}
	.shopp-nav-list-shop{
		height: 442rpx;
	}
	.shopp-nav-list-img{
		width: 334rpx;
		height: 334rpx;
		margin-right: 22rpx;
	}
	.shopp-nav-list-text1{
		width: 338rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
		margin-top: 14rpx;
	}
	.shopp-nav-list-text2{
		width: 138rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #C80000;
		line-height: 38rpx;
		margin-top: 10rpx;
	}
	.shopp-nav-bottom{
		margin-top: 20rpx;
		width: 100%;
		height: 112rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
	}
	.shopp-information{
		width: 100%;
		height: 2222rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
	}
	.shopp-information-product1{
		padding-top: 30rpx;
		margin-left: 30rpx;
		width: 128rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 38rpx;
	}
	.shopp-information-product2{
		width: 532rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
		margin-top: 16rpx;
		margin-left: 30rpx;
	}
	.shopp-information-product3{
		width: 128rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 38rpx;
		margin-top: 16rpx;
		margin-left: 30rpx;
	}
	.shopp-information-product4{
		width: 672rpx;
		height: 120rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 38rpx;
		margin-top: 16rpx;
		margin-left: 30rpx;
	}
	.shopp-information-product5{
		width: 690rpx;
		height: 72rpx;
		background: #F5F5F5;
		border-radius: 12rpx 12rpx 12rpx 12rpx;
		opacity: 1;
		margin-top: 30rpx;
		margin-left: 30rpx;
		text-align: center;
		line-height: 72rpx;
		color: #3891ED;
		font-family: PingFang SC-Regular;
		font-weight: Regular;
		font-size: 28rpx;
	}
	.shopp-information-product6{
		width: 160rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 38rpx;
		margin-top: 30rpx;
		margin-left: 30rpx;
	}
	.shopp-information-product7{
		width: 108rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
		margin-left: 30rpx;
		margin-top: 16rpx;
	}
	.shopp-information-product8{
		width: 128rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 38rpx;
		margin-left: 30rpx;
		margin-top: 30rpx;
	}
	.shopp-contact{
		width: 100%;
		height: 168rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		margin-top: 20rpx;
	}
	.shopp-contact-text1{
		width: 128rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 38rpx;
		padding-top: 30rpx;
		margin-left: 30rpx;
	}
	.shopp-contact-text2{
		display: flex;
		margin-left: 30rpx;
		margin-top: 20rpx;
	}
	.shopp-contact-text2-phone{
		width: 316rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 38rpx;
	}
	.shopp-contact-text2-img{
		width: 48rpx;
		height: 48rpx;
		margin-left: 326rpx;
	}
</style>