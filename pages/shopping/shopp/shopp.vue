<template>
	<view class="shopp">
		<view class="shopp-top">
			<view class="shopp-hz">
				<view>
					<view class="shopp-top-left">
						扯的店铺，这是一家神奇的店铺
					</view>
					<image class="shopp-top-left-img" src="../../../static/img/qiye.png" mode=""></image>
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
				<u-tabs class="shopp-nav1-tabs" :list="list1" @change="qhclick"></u-tabs>
			</view>
				  <view class="shopp-nav-list" v-if="active == 1">
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
				  <view class="shopp-nav-bottom" v-else>
				  	
				  </view>
			
		</view>
		
	</view>
</template>

<script>
	export default {
		data() {
			return {
				active:1,
				list1:[{name:'公司信息'},{name:'供应商品'}],
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
		display: flex;
		justify-content: space-around;
	}
	.shopp{
		width: 100%;
		height: 1774rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.shopp-top{
		width: 100%;
		height: 314rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
	}
	.shopp-top2{
		padding: 0 30rpx;
		margin-top: 36rpx;
		margin-bottom: 20rpx;
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
	}
	.shopp-top-right-img{
		margin-left: 118rpx;
		margin-top: 30rpx;
		width: 124rpx;
		height: 124rpx;
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
</style>