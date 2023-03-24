<template>
	<view>
		<view class="inquiry_center">
			<view class="inquiry_center_text1">
				猪产品 100千克 | 现货
			</view>
			<view class="inquiry_center_text2">
				生产国家：中国、韩国
			</view>
			<view class="inquiry_center_text3">
				要货时间：2022年12月12日 11:00前
			</view>
			<view class="inquiry_center_text3">
				收货地区：北京丰台区
			</view>
			<view class="inquiry_center_text3">
				报价（不）含税（不）含运费
			</view>
			<view class="inquiry_center_text3">
				允许报价方来电：是
			</view>
			<view class="inquiry_center_text3">
				发布时间：2022年12月12日 11:00
			</view>
		</view>
		<view class="inquiry_buyShopp">
			
		</view>
		<view class="box-requirements">
			<view class="box-requirements-text1">
				采购要求
			</view>
			<view class="box-requirements-text2">
				iPhone 12高度：146.7毫米；宽度：71.5毫米；厚度：7.4毫米；重量：162克（5.73盎司） [5] 。iPhone 12设计采用了离子玻璃，以及7000系列铝金属外壳。iPhone 12采用了直面边框设计，背部颜色有：黑色、白色、红色、绿色、蓝色、紫色 [2] 。
			</view>
			<image class="box-requirements-img" src="../../static/img/jing.png" mode=""></image>
		</view>
		<!-- <view class="inquiry_bottom">
			<view class="inquiry_bottom_top">
				<view class="inquiry_bottom_top_text1">
					实力卖家推荐
				</view>
				<view class="inquiry_bottom_top_text2">
					（根据买家询价单的筛选条件来匹配有货的商家）
				</view>
			</view>
			<view class="inquiry_bottom_list" v-for="(item,index) in list" :key="index">
				<image class="inquiry_bottom_list_img" :src="item.url" mode=""></image>
				<view class="inquiry_bottom_list_text">
					<view class="inquiry_bottom_list_text_t1">
						{{item.text1}}
					</view>
					<view class="inquiry_bottom_list_text_t2">
						<view class="inquiry_bottom_list_text_t2_text1">
							访问店铺
						</view>
						<view class="inquiry_bottom_list_text_t2_text2">
							邀请报价
						</view>
					</view>
				</view>
			</view>
			<view class="inquiry_bottom_list_text2">
				更多
			</view>
		</view> -->
	</view>
</template>

<script>
	export default{
		data(){
			return {
				list:[
					{
						url:'../../static/img/tupian.png',
						text1:'黑龙江哈尔滨食品有限公司'
					},
					{
						url:'../../static/img/tupian.png',
						text1:'黑龙江哈尔滨食品有限公司'
					},
					{
						url:'../../static/img/tupian.png',
						text1:'黑龙江哈尔滨食品有限公司'
					}
				]
			}
		}
	}
</script>

<style>
	.inquiry{
		height: 3120rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		position: relative;
	}
	.inquiry_center{
		height: 424rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		padding: 30rpx;
		margin-bottom: 20rpx;
	}
	.inquiry_center_text1{
		height: 74rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 38rpx;
		border-bottom: 2rpx solid #f8f8f8;
	}
	.inquiry_center_text2{
		margin-top: 30rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
	}
	.inquiry_center_text3{
		margin-top: 16rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
	}
	.inquiry_buyShopp{
		height: 432rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		margin-bottom: 20rpx;
	}
	.box-requirements{
		width: 100%;
		height: 770rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		margin-bottom: 20rpx;
	}
	.box-requirements-text1{
		padding-top: 30rpx;
		margin-left: 40rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 38rpx;
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
	/* .inquiry_bottom{
		height: 648rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		padding: 32rpx 6rpx 32rpx 30rpx;
	}
	.inquiry_bottom_top{
		display: flex;
		height: 44rpx;
		align-items: center;
	}
	.inquiry_bottom_top_text1{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 38rpx;
		white-space:nowrap;
	}
	.inquiry_bottom_top_text2{
		height: 34rpx;
		font-size: 24rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
		line-height: 28rpx;
		white-space:nowrap;
	}
	.inquiry_bottom_list{
		height: 144rpx;
		margin-right: 24rpx;
		border-bottom: 2rpx solid #f8f8f8;
		display: flex;
		margin-top: 36rpx;
	}
	.inquiry_bottom_list_img{
		width: 112rpx;
		height: 112rpx;
	}
	.inquiry_bottom_list_text{
		margin-left: 20rpx;
	}
	.inquiry_bottom_list_text_t1{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 38rpx;
	}
	.inquiry_bottom_list_text_t2{
		margin-top: 20rpx;
		display: flex;
	}
	.inquiry_bottom_list_text_t2_text1{
		width: 160rpx;
		height: 52rpx;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		border: 2rpx solid #999999;
		font-size: 24rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 52rpx;
		text-align: center;
	}
	.inquiry_bottom_list_text_t2_text2{
		margin-left: 10rpx;
		width: 160rpx;
		height: 52rpx;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		border: 2rpx solid #999999;
		font-size: 24rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 52rpx;
		text-align: center;
	}
	.inquiry_bottom_list_text2{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
		text-align: center;
		margin-top: 30rpx;
	} */
</style>