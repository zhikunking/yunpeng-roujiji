<template>
	<view>
					<view class="submit-shop">
						<view v-for="(item,index) in list1" :key="index">
							<view class="submit-shop-text1">
								{{item.name1}}
							</view>
							<view class="submit-shop-text2">
								{{item.name2}}
							</view>
						</view>
						<view class="submit-shop-list" v-for="(item,index) in list2" :key="index">
							<image class="submit-shop-list-img" :src="item.url" mode=""></image>
							<view class="submit-shop-list-right">
								<view class="submit-shop-list-right-text1">
									{{item.name3}}
								</view>
								<view class="submit-shop-list-right-text2">
									{{item.name4}}
								</view>
								<view class="submit-shop-list-right-text3">
									<view class="submit-shop-list-right-text4">
										{{item.name5}}
									</view>
									<view class="submit-shop-list-right-text5">
										<u-number-box v-model="value" @change="valChange"></u-number-box>
									</view>
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
			value:0,
		  list1:[
				{
				name1:'JD Apple 产品京东自营旗舰店',
				name2:'店铺起售量：200千克'
			},
		  ],
		  list2:[
		  				{
		  				name3:'猪肉-SKU名称',
		  				name4:'鲜品-中国-国家101厂',
		  				name5:'￥99.99',
		  				url:'../../static/img/root2.png'
		  			},
					{
						name3:'猪肉-SKU名称',
						name4:'鲜品-中国-国家101厂32',
						name5:'￥9999.99',
						url:'../../static/img/root2.png'
					},
		  ]
	    };
	  },
	  methods:{
		  valChange(e) {
		  				console.log('当前值为: ' + e.value)
		  			}
		  
	  }
	};
</script>

<style>
	.submit-shop{
		height: 472rpx;
		background: #FFFFFF;
		opacity: 1;
	}
	.submit-shop-text1{
		width: 400rpx;
		padding-top: 20rpx;
		margin-left: 32rpx;
		width: 436rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 38rpx;
	}
	.submit-shop-text2{
		width: 276rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
		line-height: 32rpx;
		margin-left: 32rpx;
	}
	.submit-shop-list{
		display: flex;
		margin-top: 22rpx;
		margin-left: 32rpx;
	}
	.submit-shop-list-img{
		width: 148rpx;
		height: 148rpx;
	}
	.submit-shop-list-right{
		margin-left: 32rpx;
	}
	.submit-shop-list-right-text1{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 38rpx;
	}
	.submit-shop-list-right-text2{
		height: 34rpx;
		font-size: 24rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #666666;
		line-height: 28rpx;
		margin-top: 8rpx;
	}
	.submit-shop-list-right-text3{
		display: flex;
		margin-top: 10rpx;
	}
	.submit-shop-list-right-text4{
		width: 118rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #C80000;
		line-height: 38rpx;
		margin-right: 164rpx;
	}
	.submit-shop-list-right-text5{
		margin-right:32rpx ;
	}
</style>