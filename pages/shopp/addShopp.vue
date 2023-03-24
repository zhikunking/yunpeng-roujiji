<template>
	<view class="box">
		<view class="box-top">
			<image class="box-top-img" src="../../static/img/jinggao2.png"></image>
			<view class="box-top-text">
				<p>温馨提示：</p>
				系统默认您此处添加的产品是单批采购，对于单个商家的多产品报价，您只能整体采纳他的报价，所以请您将需要单批一起采购的商品采用单询价单多商品模式。
			</view>
		</view>
		<view class="box-shoppName">
			<view class="my-tousu-list-yi">
				<view class="my-tousu-list-yi-text1">商品名称</view>
				<view class="my-tousu-list-yi-text2">名称</view>
			</view>
			<view class="my-tousu-list-yi">
				<view class="my-tousu-list-yi-text1">鲜冻类型</view>
				<view class="my-tousu-list-yi-text2">不限</view>
			</view>
			<view class="my-tousu-list-yi">
				<view class="my-tousu-list-yi-text1">采购数量</view>
				<view class="my-tousu-list-yi-t1">
					<view class="my-tousu-list-yi-text2">
						1000
					</view>
					<view class="my-tousu-list-yi-text3">
						<view class="my-tousu-list-yi-text4">
							千克
						</view>
						<image class="my-tousu-list-yi-text5" src="../../static/img/xia2.png" mode=""></image>
					</view>
				</view>
			</view>
			<view class="my-tousu-list-er">
				<image class="my-tousu-list-er-img" src="../../static/img/del4.png" mode=""></image>
				<view class="my-tousu-list-er-text">
					删除
				</view>
			</view>
		</view>
		<view class="box-shoppName2">
			<view class="my-tousu-list-yi">
				<view class="my-tousu-list-yi-text1">商品名称</view>
				<input class="box-shoppName2-text2" placeholder="请输入"/>
			</view>
			<view class="box-shoppName2-yi">
				<view class="box-shoppName2-yi-text1">
					鲜冻类型
				</view>
				<image class="box-shoppName2-yi-img1" src="../../static/img/yuan2.png" mode=""></image>
				<!-- <image class="box-shoppName2-yi-img1" src="../../static/img/yuan1.png" mode=""></image> -->
				<view class="box-shoppName2-yi-text2">
					鲜品
				</view>
				<image class="box-shoppName2-yi-img2" src="../../static/img/yuan1.png" mode=""></image>
				<!-- <image class="box-shoppName2-yi-img2" src="../../static/img/yuan2.png" mode=""></image> -->
				<view class="box-shoppName2-yi-text2">
					冻品
				</view>
				<image class="box-shoppName2-yi-img2" src="../../static/img/yuan1.png" mode=""></image>
				<!-- <image class="box-shoppName2-yi-img2" src="../../static/img/yuan2.png" mode=""></image> -->
				<view class="box-shoppName2-yi-text2">
					不限
				</view>
			</view>
			<view class="my-tousu-list-yi">
				<view class="my-tousu-list-yi-text1">采购数量</view>
				<view class="my-tousu-list-yi-t1">
					<view class="my-tousu-list-yi-text2">
						1000
					</view>
					<view class="my-tousu-list-yi-text3">
						<view class="my-tousu-list-yi-text4">
							千克
						</view>
						<image class="my-tousu-list-yi-text5" src="../../static/img/xia2.png" mode=""></image>
					</view>
				</view>
			</view>
		</view>
		<view class="box-btn">
			<view class="box-btn-text1">
				+
			</view>
			<view class="box-btn-text2">
				再添加一条商品
			</view>
		</view>
		<view class="enquiryShopp-bottom">
			<view class="enquiryShopp-bottom-btn">
				保存
			</view>
		</view>
	</view>
</template>

<script>
	export default{
		data(){
			return{
				
			}
		}
	}
</script>

<style>
	.box{
		height: 1424rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		position: relative;
	}
	.box-top{
		width: 750rpx;
		height: 178rpx;
		background: #F05904;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 0.1;
		display: flex;
	}
	.box-top-img{
		width: 36rpx;
		height: 36rpx;
		margin-top: 20rpx;
		margin-left: 30rpx;
	}
	.box-top-text{
		width: 650rpx;
		height: 136rpx;
		font-size: 24rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #DF0202;
		line-height: 34rpx;
		margin-top: 18rpx;
		margin-left: 2rpx;
	}
	.box-shoppName{
		margin-top: 16rpx;
		margin-left: 30rpx;
		width: 694rpx;
		height: 456rpx;
		background: #FFFFFF;
		border-radius: 20rpx 20rpx 20rpx 20rpx;
		opacity: 1;
	}
	.my-tousu-list-yi{
		height: 120rpx;
		margin: 0 30rpx;
		border-bottom: 2rpx solid #f8f8f8;
		display: flex;
		align-items: center;
		justify-content: space-between;
	}
	.my-tousu-list-yi-text1{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 38rpx;
		line-height: 38rpx;
	}
	.my-tousu-list-yi-text2{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
		margin-right: 20rpx;
		margin-top: 6rpx;
	}
	.my-tousu-list-yi-text3{
		width: 120rpx;
		height: 48rpx;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		border: 2rpx solid #C1C1C1;
		
		display: flex;
		align-items: center;
		/* justify-content: center; */
	}
	.my-tousu-list-yi-text4{
		width: 56rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #C1C1C1;
		line-height: 33rpx;
		margin-left: 16rpx;
	}
	.my-tousu-list-yi-text5{
		width: 32rpx;
		height: 32rpx;
	}
	.my-tousu-list-yi-t1{
		width: 220rpx;
		display: flex;
		align-items: center;
	}
	.my-tousu-list-er{
		height: 94rpx;
		display: flex;
		align-items: center;
		justify-content: center;
	}
	.my-tousu-list-er-img{
		width: 48rpx;
		height: 48rpx;
	}
	.my-tousu-list-er-text{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #DC0000;
		line-height: 38rpx;
		margin-left: 10rpx;
	}
	.box-shoppName2{
		width: 694rpx;
		height: 350rpx;
		background: #FFFFFF;
		border-radius: 20rpx 20rpx 20rpx 20rpx;
		opacity: 1;
		margin-top: 20rpx;
		margin-left: 30rpx;
	}
	.box-shoppName2-text2{
		width: 84rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
		line-height: 33rpx;
	}
	.box-shoppName2-yi{
		height: 120rpx;
		border-bottom: 2rpx solid #f8f8f8;
		margin: 0 30rpx;
		display: flex;
		align-items: center;
	}
	.box-shoppName2-yi-text1{
		width: 128rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 38rpx;
	}
	.box-shoppName2-yi-img1{
		width: 56rpx;
		height: 56rpx;
		margin-left: 112rpx;
	}
	.box-shoppName2-yi-text2{
		margin-left: 6rpx;
		width: 56rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
		margin-top: 6rpx;
	}
	.box-shoppName2-yi-img2{
		margin-left: 8rpx;
		width: 56rpx;
		height: 56rpx;
	}
	.box-shoppName2-er{
		height: 120rpx;
		display: flex;
		align-items: center;
	}
	.box-shoppName2-er-text{
		width: 128rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 38rpx;
		margin-left: 30rpx;
	}
	.box-btn{
		width: 300rpx;
		height: 72rpx;
		border-radius: 12rpx 12rpx 12rpx 12rpx;
		opacity: 1;
		border: 2rpx solid #999999;
		line-height: 72rpx;
		margin: 0 auto;
		margin-top: 34rpx;
		display: flex;
		align-items: center;
		justify-content: center;
	}
	.box-btn-text1{
		width: 30rpx;
		height: 78rpx;
		font-size: 48rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 56rpx;
	}
	.box-btn-text2{
		width: 196rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
		margin-left: 12rpx;
	}
	.enquiryShopp-bottom{
		position: absolute;
		width: 100%;
		bottom: 0;
		height: 120rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
	}
	.enquiryShopp-bottom-btn{
		width: 690rpx;
		height: 88rpx;
		line-height: 88rpx;
		text-align: center;
		background: #3891ED;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		margin-top: 16rpx;
		margin-left: 30rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #FFFFFF;
	}
</style>