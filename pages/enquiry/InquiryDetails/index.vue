<template>
	<view class="box">
		<view class="box-top">
			<u-cell-group>
					<u-cell>
						<template #title>
							<view class="box-top-text1">鸡产品100千克 | 现货</view>
						</template>
					</u-cell>
					<u-cell>
						<template #title>
							<view class="box-top-text2">生产国家：中国、韩国</view>
							<view class="box-top-text3">要货时间：2022年12月12日11:00前</view>
							<view class="box-top-text3">收货地址：北京丰台区</view>
							<view class="box-top-text3">报价（不）含税（不）含运费</view>
							<view class="box-top-text3">发布时间：2022年12月12日11:00</view>
						</template>
					</u-cell>
				</u-cell-group>
		</view>
		<view class="box-btn1">
			<view class="box-btn2">
				<view class="box-btn2-text1">
					<view class="box-btn2-text1-t1">
						0
					</view>
					<view class="box-btn2-text1-t2">
						待选商
					</view>
				</view>
				<view class="box-btn2-text1">
					<view class="box-btn2-text1-t1">
						0
					</view>
					<view class="box-btn2-text1-t2">
						已成交
					</view>
				</view>
			</view>
		</view>
		<view class="box-shopp">
			<u-cell-group>
				<u-cell>
					<template #title>
						<view class="box-shopp-text1">采购商品</view>
					</template>
				</u-cell>
			  <u-cell>
			  	<template #title>
			  	
			  	</template>
			  </u-cell>
			</u-cell-group>
		</view>
		<view class="box-requirements">
			<view class="box-requirements-text1">
				采购要求
			</view>
			<view class="box-requirements-text2">
				iPhone 12高度：146.7毫米；宽度：71.5毫米；厚度：7.4毫米；重量：162克（5.73盎司） [5] 。iPhone 12设计采用了离子玻璃，以及7000系列铝金属外壳。iPhone 12采用了直面边框设计，背部颜色有：黑色、白色、红色、绿色、蓝色、紫色 [2] 。
			</view>
			<image class="box-requirements-img" src="../../../static/img/jing.png" mode=""></image>
		</view>
		<view class="info-shop-information">
			<u-cell-group>
			  <u-cell>
				  <template #title>
					  <view class="info-shop-information-text">
							<view class="info-shop-information-text1">询价人</view>
							<view class="info-shop-information-text2">私聊</view>
							<image class="info-shop-information-text3" src="../../../static/img/right.png" mode=""></image>
					  </view>
				  </template>
			  </u-cell>
			  <!-- <u-cell>
				  <template #title>
				  	<view class="info-shop-information-img">
						<view>
							<image class="info-shop-information-img1" src="../../../static/img/tupian.png"></image>
						</view>
						<view>
							<view class="info-shop-information-img2">黑龙江哈尔滨食品有限公司</view>
							<view class="info-shop-information-img3">
								<image class="info-shop-information-img4" src="../../../static/img/qiye.png" mode=""></image>
								<image class="info-shop-information-img4" src="../../../static/img/geren.png" mode=""></image>
								<image class="info-shop-information-img4" src="../../../static/img/geti.png" mode=""></image>
							</view>
						</view>
					</view>
					<view class="info-shop-information-t1">
						注册时间：2022年11月10日 累计询价100次
					</view>
				  </template>
			  </u-cell> -->
			  <u-cell>
			  				  <template #title>
			  				  	<view class="info-shop-information-img">
			  						<view>
			  							<image class="info-shop-information-img1" src="../../../static/img/tupian.png"></image>
			  						</view>
			  						<view>
			  							<view class="info-shop-information-img2">王小明</view>
			  							<view class="info-shop-information-img3">
			  								<image class="info-shop-information-img4" src="../../../static/img/shiming.png" mode=""></image>
			  							</view>
			  						</view>
			  					</view>
			  					<view class="info-shop-information-t1">
			  						注册时间：2022年11月10日 累计询价100次
			  					</view>
			  				  </template>
			  </u-cell>
			</u-cell-group>
		</view>
	</view>
</template>

<script>
	export default {}
</script>

<style>
	.box{
		width: 100%;
		height: 2366rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.box-top{
		width: 100%;
		height: 398rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
	}
	.box-top-text1{
		width: 330rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 38rpx;
		padding-top: 30rpx;
		margin-left: 30rpx;
	}
	.box-top-text2{
		width: 280rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
		margin-top: 20rpx;
		margin-left: 30rpx;
	}
	.box-top-text3{
		width: 460rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
		margin-top: 10rpx;
		margin-left: 30rpx;
	}
	.box-btn1{
		width: 100%;
		height: 194rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		padding-top: 40rpx;
	} 
	.box-btn2{
		width: 650rpx;
		height: 144rpx;
		background: #F5F5F5;
		border-radius: 20rpx 20rpx 20rpx 20rpx;
		margin-left: 50rpx;
		padding-top: 20rpx;
		display: flex;
		align-items: center;
		justify-content: space-around;
	}
	.box-btn2-text1{
		width: 104rpx; 
	}
	.box-btn2-text1-t1{
		width: 104rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 38rpx;
		text-align: center;
	}
	.box-btn2-text1-t2{
		width: 104rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
		text-align: center;
	}
	.box-shopp{
		width: 100%;
		height: 432rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		margin-top: 20rpx;
	}
	.box-shopp-text1{
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
	.box-requirements{
		width: 100%;
		height: 770rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		margin-top: 20rpx;
	}
	.box-requirements-text1{
		padding-top: 30rpx;
		margin-left: 40rpx;
	}
	.box-requirements-text2{
		margin-left: 40rpx;
		margin-top: 20rpx;
		width: 670rpx;
		height: 208rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 40rpx;
	}
	.box-requirements-img{
		width: 670rpx;
		height: 400rpx;
		margin-top: 28rpx;
		margin-left: 40rpx;
	}
	.info-shop-information{
		margin-top: 20rpx;
		width: 100%;
		height: 314rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
	}
	.info-shop-information-text{
		display: flex;
	}
	.info-shop-information-text1{
		width: 128rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 38rpx;
	}
	.info-shop-information-text2{
		width: 56rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #3891ED;
		line-height: 33rpx;
		margin-left: 230px;
		margin-top: 10rpx;
	}
	.info-shop-information-text3{
		width: 36rpx;
		height: 36rpx;
		margin-top: 9rpx;
	}
	.info-shop-information-img{
		display: flex;
	}
	.info-shop-information-img1{
		width: 112rpx;
		height: 112rpx;
		margin-left: 20rpx;
	}
	.info-shop-information-img2{
		margin-left: 20rpx;
		width: 384rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 38rpx;
	}
	.info-shop-information-img3{
		margin-left: 20rpx;
	}
	.info-shop-information-img4{
		width: 92rpx;
		height: 50rpx;
		margin-top: 10rpx;
		margin-right: 20rpx;
	}
	.info-shop-information-t1{
		margin-left: 150rpx;
		width: 556rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
		line-height: 33rpx;
	}
</style>