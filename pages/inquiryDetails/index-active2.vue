<template>
	<view>
		<view class="inquiry_bottom">
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
		</view>
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
	.inquiry_bottom{
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
	}
</style>