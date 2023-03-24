<template>
	<view class="send">
		<view class="send-yi">
			<view class="send-yi-text1">
				商品类别
			</view>
			<view class="send-yi-text2">
				<view class="send-yi-text2-t1">
					请选择
				</view>
				<image class="send-yi-text2-img" src="../../static/img/right2.png" mode=""></image>
			</view>
		</view>
		<view class="box-shoppName2-yi">
			<view class="box-shoppName2-yi-text1">
				商品状态
			</view>
			<image class="box-shoppName2-yi-img1" src="../../static/img/yuan2.png" mode=""></image>
			<!-- <image class="box-shoppName2-yi-img1" src="../../static/img/yuan1.png" mode=""></image> -->
			<view class="box-shoppName2-yi-text2">
				提货
			</view>
			<image class="box-shoppName2-yi-img2" src="../../static/img/yuan1.png" mode=""></image>
			<!-- <image class="box-shoppName2-yi-img2" src="../../static/img/yuan2.png" mode=""></image> -->
			<view class="box-shoppName2-yi-text2">
				期货
			</view>
			<image class="box-shoppName2-yi-img2" src="../../static/img/yuan1.png" mode=""></image>
			<!-- <image class="box-shoppName2-yi-img2" src="../../static/img/yuan2.png" mode=""></image> -->
			<view class="box-shoppName2-yi-text2">
				不限
			</view>
		</view>
		<view class="box-shoppName2-yi">
			<view class="box-shoppName2-yi-text1">
				公母类型
			</view>
			<image class="box-shoppName2-yi-img1" src="../../static/img/yuan2.png" mode=""></image>
			<!-- <image class="box-shoppName2-yi-img1" src="../../static/img/yuan1.png" mode=""></image> -->
			<view class="box-shoppName2-yi-text2">
				公
			</view>
			<image class="box-shoppName2-yi-img2" src="../../static/img/yuan1.png" mode=""></image>
			<!-- <image class="box-shoppName2-yi-img2" src="../../static/img/yuan2.png" mode=""></image> -->
			<view class="box-shoppName2-yi-text2">
				母
			</view>
			<image class="box-shoppName2-yi-img2" src="../../static/img/yuan1.png" mode=""></image>
			<!-- <image class="box-shoppName2-yi-img2" src="../../static/img/yuan2.png" mode=""></image> -->
			<view class="box-shoppName2-yi-text2">
				不限
			</view>
		</view>
		<view class="cell">
		    <view class="cell__title">生产国家(可多选)</view>
			<image class="cell__img" src="../../static/img/yuan2.png" mode=""></image>
			<view class="cell__text">国内</view>
			<image class="cell__img1" src="../../static/img/yuan1.png" mode=""></image>
			<view class="cell__text">不限</view>
			<view class="cell__text1">
				更多
			</view>
		</view>
		<view class="cell2">
			<view class="cell2_title">
				添加商品
			</view>
			<view class="cell2_text">
				<view class="cell2_text-t1">
					请添加商品
				</view>
				<image class="cell2_text-img" src="../../static/img/right2.png" mode=""></image>
			</view>
		</view>
		<view class="cell3">
			<view class="cell2_title">
				采购要求（可不填）
			</view>
			<view class="cell2_text">
				<view class="cell2_text-t1">
					补充描述/上述图片
				</view>
				<image class="cell2_text-img" src="../../static/img/right2.png" mode=""></image>
			</view>
		</view>
		<view class="cell3">
			<view class="cell2_title">
				收获地区
			</view>
			<view class="cell2_text">
				<view class="cell2_text-t1">
					定位
				</view>
				<image class="cell2_text-img" src="../../static/img/right2.png" mode=""></image>
			</view>
		</view>
		<view class="cell3">
			<view class="cell2_title">
				要货时间
			</view>
			<view class="cell2_text">
				<view class="cell2_text-t1">
					请选择要货时间
				</view>
				<image class="cell2_text-img" src="../../static/img/right2.png" mode=""></image>
			</view>
		</view>
		<view class="cell2">
			<view class="cell2_title">
				允许报价商来电
			</view>
			<view class="cell2_text">
				<u-switch v-model="value" @change="isShow"></u-switch>
				<image class="cell2_text-img" src="../../static/img/right2.png" mode=""></image>
			</view>
		</view>
		<view class="cell3">
			<view class="cell2_title">
				报价是否含运费
			</view>
			<view class="cell2_text">
				<u-switch v-model="value2" @change="isShow"></u-switch>
				<image class="cell2_text-img" src="../../static/img/right2.png" mode=""></image>
			</view>
		</view>
		<view class="cell4">
			<view class="cell2_title">
				报价是否含税
			</view>
			<view class="cell2_text">
				<u-switch v-model="value2" @change="isShow"></u-switch>
				<image class="cell2_text-img" src="../../static/img/right2.png" mode=""></image>
			</view>
		</view>
		<view class="enquiryShopp-bottom">
			<view class="enquiryShopp-bottom-btn">
				确认提交
			</view>
		</view>
	</view>
</template>

<script>
	export default {
	    data(){
			return{
				value:true,
				value2:false
			}
		},
		methods:{
			isShow(){
				console.log(e);
			}
		}
	  }
</script>

<style>
	.send{
		height: 1374rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		position: relative;
	}
	.send-yi{
		height: 104rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		border-bottom: 2rpx solid #e5e5e5;
		display: flex;
		align-items: center;
		justify-content: space-between;
		padding: 0 30rpx;
	}
	.send-yi-text1{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 38rpx;
	}
	.send-yi-text2{
		display: flex;
		align-items: center;
	}
	.send-yi-text2-t1{
		width: 84rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
		line-height: 33rpx;
	}
	.send-yi-text2-img{
		width: 40rpx;
		height: 40rpx;
		margin-top: -8rpx;
	}
	.box-shoppName2-yi{
		height: 104rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		border-bottom: 2rpx solid #e5e5e5;
		display: flex;
		align-items: center;
		justify-content: space-between;
		padding: 0 30rpx;
	}
	.box-shoppName2-yi-text1{
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
	.cell {
	    display: flex;
	    flex-direction: row;
	    align-items: center;
		height: 104rpx;
	    padding: 0 30rpx;
		background: #FFFFFF;
	  }
	  .cell__title {
	    font-size: 32rpx;
	    color: #333333;
	    line-height: 100px;
	  }
	.cell__img{
		width: 56rpx;
		height: 56rpx;
		margin-left: 8rpx;
	}
	.cell__text{
		margin-left: 16rpx;
		margin-bottom: 6rpx;
	}
	.cell__img1{
		width: 56rpx;
		height: 56rpx;
		margin-left: 16rpx;
	}
	.cell__text1{
		width: 56rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #3891ED;
		line-height: 33rpx;
		margin-top: 6rpx;
		margin-left: 82rpx;
	}
	.cell2{
		height: 104rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		margin-top: 20rpx;
		display: flex;
		align-items: center;
		justify-content: space-between;
		padding: 0 30rpx;	    
		border-bottom: 2rpx solid #e5e5e5;
	}
	.cell2_title{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 38rpx;
	}
	.cell2_text{
		display: flex;
		align-items: center;
	}
	.cell2_text-t1{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
		line-height: 33rpx;
	}
	.cell2_text-img{
		width: 40rpx;
		height: 40rpx;
		margin-bottom: 8rpx;
		margin-left: 8rpx;
	}
	.cell3{
		height: 104rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		display: flex;
		align-items: center;
		justify-content: space-between;
		padding: 0 30rpx;	    
		border-bottom: 2rpx solid #e5e5e5;
	}
	.cell4{
		height: 104rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		display: flex;
		align-items: center;
		justify-content: space-between;
		padding: 0 30rpx;	    
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