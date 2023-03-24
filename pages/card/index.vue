<template>
	<view class="card">
		<view class="card-box1"></view>
		<view>
			<view class="card-box-t1" v-for="(item,index) in list1" :key="index">
				<image class="card-box-t1-img" :src="item.url1" mode=""></image>
				<!-- <image class="card-box-t1-img" :src="item.url2" mode=""></image> -->
				<view class="card-box-t2">
					<view class="card-box-t2-text1">
						{{item.text4}}
					</view>
					<view class="card-box-t2-text2">
						{{item.text5}}
					</view>
				</view>
				<image class="card-box-t2-img" :src="item.url3" mode=""></image>
				<image class="card-box-t3" :src="item.url4"></image>
			</view>
			<view class="card-box2" v-for="(item,index) in list" :key="index">
				<image class="card-box2-t1" :src="item.url1"></image>
				<!-- <image class="card-box2-t1" :src="item.url2"></image> -->
				<image class="card-box2-t2" :src="item.url5"></image>
				<view class="card-box2-t3">
					<view class="card-box2-t3-text1">
						{{item.text1}}
					</view>
					<view class="card-box2-t3-text2">
						{{item.text2}}
					</view>
					<view class="card-box2-t3-text3">
						{{item.text3}}
					</view>
				</view>
				<view class="card-box2-t4">
					<u-number-box v-model="value" @change="valChange"></u-number-box>
				</view>
			</view>
		</view>
		<view class="card-bottom">
			<view class="card-bottom1">
				<image class="card-bottom1-img" src="../../static/img/jianggao.png" mode=""></image>
				<view class="card-bottom1-text">
					还差490公斤可下单，您可以再选购该店铺其他商品
				</view>
			</view>
			<view class="card-bottom2">
				<image class="card-bottom2-img" src="../../static/img/yuan1.png" mode=""></image>
				<view class="card-bottom2-text">
					全选   合计：￥100.00
				</view>
				<view class="card-bottom2-btn">
					去结算（0）
				</view>
			</view>
		</view>
	</view>
</template>

<script>
	export default{
		data(){
			return{
				value:0,
				list:[
					{
						url1:'../../static/img/yuan1.png',
						url2:'../../static/img/yuan2.png',
						url5:'../../static/img/root2.png',
						text1:'猪肉-SKU名称',
						text2:'鲜品-中国-国家101厂',
						text3:'￥99.99'
					},
					{
						url1:'../../static/img/yuan1.png',
						url2:'../../static/img/yuan2.png',
						url5:'../../static/img/root2.png',
						text1:'猪肉-SKU名称',
						text2:'鲜品-中国-国家101厂',
						text3:'￥99.99'
					},
					{
						url1:'../../static/img/yuan1.png',
						url2:'../../static/img/yuan2.png',
						url5:'../../static/img/root2.png',
						text1:'猪肉-SKU名称',
						text2:'鲜品-中国-国家101厂',
						text3:'￥99.99'
					},
				],
				list1:[
					{
						url3:'../../static/img/shangbiao.png',
						url4:'../../static/img/Group422.png',
						text4:'JD Apple 产品京东自营旗舰店',
						text5:'店铺起售量：200千克',
						url1:'../../static/img/yuan1.png',
						url2:'../../static/img/yuan2.png'
					}
				]
			}
		},
		methods: {
					valChange(e) {
						console.log('当前值为: ' + e.value)
					}
				}
	}
</script>

<style>
	.card{
		height: 1424rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		position: relative;
	}
	.card-box1{
		width: 100%;
		height: 20rpx;
		background: #F5F5F5;
	}
	.card-box-t1{
		height: 104rpx;
		background: #FFFFFF;
		/* padding-top: 10rpx; */
		display: flex;
		align-items: center;
	}
	.card-box-t1-img{
		width: 56rpx;
		height: 56rpx;
		margin-left: 24rpx;
	}
	.card-box-t2{
		margin-left: 20rpx;
	}
	.card-box-t2-text1{
		width: 436rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 38rpx;
	}
	.card-box-t2-text2{
		width: 276rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
		line-height: 33rpx;
	}
	.card-box-t2-img{
		width: 36rpx;
		height: 36rpx;
		margin-left: 12rpx;
		margin-top: -40rpx;
	}
	.card-box-t3{
		width: 92rpx;
		height: 50rpx;
		margin-top: -40rpx;
		margin-left: 44rpx;
	}
	.card-box2{
		display: flex;
		align-items: center;
		height: 168rpx;
		background: #FFFFFF;
		padding-bottom: 20rpx;
	}
	.card-box2-t1{
		width: 56rpx;
		height: 56rpx;
		margin-left: 24rpx;
	}
	.card-box2-t2{
		width: 148rpx;
		height: 148rpx;
		margin-left: 20rpx;
	}
	.card-box2-t3{
		margin-left: 20rpx;
	}
	.card-box2-t3-text1{
		width: 216rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 38rpx;
		margin-top: -10rpx;
		margin-bottom: 8rpx;
	}
	.card-box2-t3-text2{
		width: 232rpx;
		height: 34rpx;
		font-size: 24rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #666666;
		line-height: 28rpx;
		margin-bottom: 10rpx;
	}
	.card-box2-t3-text3{
		width: 118rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #C80000;
		line-height: 38rpx;
	}
	.card-box2-t4{
		margin-top: 90rpx;
	}
	.card-bottom{
		width: 100%;
		height: 174rpx;
		position: absolute;
		bottom: 0;
	}
	.card-bottom1{
		display: flex;
		align-items: center;
		height: 62rpx;
		background: #FFE4D5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
	}
	.card-bottom1-img{
		margin-left: 30rpx;
		width: 34rpx;
		height: 34rpx;
	}
	.card-bottom1-text{
		width: 548rpx;
		height: 34rpx;
		font-size: 24rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #DF0202;
		line-height: 28rpx;
		margin-left: 10rpx;
	}
	.card-bottom2{
		height: 112rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		display: flex;
		align-items: center;
	}
	.card-bottom2-img{
		width: 56rpx;
		height: 56rpx;
		margin-left: 24rpx;
	}
	.card-bottom2-text{
		width: 324rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 38rpx;
		margin-left: 10rpx;
	}
	.card-bottom2-btn{
		width: 220rpx;
		height: 112rpx;
		line-height: 112rpx;
		text-align: center;
		background: #3891ED;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		margin-left: 116rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #FFFFFF;
	}
</style>