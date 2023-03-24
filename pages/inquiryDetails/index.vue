<template>
	<view class="inquiry">
		<view class="inquiry_top">
			<view class="inquiry_top_left">
				待报价
			</view>
			<view class="inquiry_top_right">
				40天后截止报价
			</view>
		</view>
		<IndexActive />
		<view class="inquiry_supplier">
			<view class="inquiry_supplier_title">
				供应商报价
			</view>
			<view class="inquiry_supplier_warn">
			<!-- 	<image class="inquiry_supplier_warn_img" src="../../static/img/jinggao2.png" mode=""></image>
				<view class="inquiry_supplier_warn_text">
					温馨提示：为了保障您的权益，肉集集建议您将和商家达成的所有约定以文字形式在平台聊天模块展现，如果和商家出现纠纷，平台会及时协助您。
				</view> -->
			</view>
			<view class="inquiry_supplier_no">
				暂未收到报价，主动邀请更快获得报价
			</view>
		</view>
		<IndexActive2 />
		<view class="inquiry_bottom2">
			<view class="inquiry_bottom2_btn1">
				修改报价单
			</view>
			<view class="inquiry_bottom2_btn2">
				停止询价
			</view>
		</view>
	</view>
</template>

<script>
	import IndexActive from "@/pages/inquiryDetails/index-active.vue"
	import IndexActive2 from "@/pages/inquiryDetails/index-active2.vue"
	export default{
		components:{
			IndexActive,
			IndexActive2
		},
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
	.inquiry_top{
		height: 44rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		padding: 30rpx;
		display: flex;
		align-items: center;
		margin-bottom: 20rpx;
	}
	.inquiry_top_left{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #C80000;
		line-height: 38rpx;
	}
	.inquiry_top_right{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		margin-left: 80rpx;
	}
	.inquiry_supplier{
		padding: 30rpx 0;
		height: 330rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		margin-bottom: 20rpx;
	}
	.inquiry_supplier_title{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 38rpx;
		margin-left: 30rpx;
	}
	.inquiry_supplier_warn{
		height: 102rpx;
		background: #F05904;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 0.1;
		margin-top: 30rpx;
		display: flex;
		padding: 20rpx 24rpx 20rpx 30rpx;
	}
	.inquiry_supplier_warn_img{
		width: 36rpx;
		height: 36rpx;
	}
	.inquiry_supplier_warn_text{
		height: 102rpx;
		font-size: 24rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #DF0202;
		line-height: 34rpx;
	}
	.inquiry_supplier_no{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #C80000;
		line-height: 38rpx;
		text-align: center;
		margin-top: 50rpx;
	}
	.inquiry_bottom2{
		position: absolute;
		bottom: 0;
		width: 100%;
		height: 104rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		display: flex;
		align-items: center;
		justify-content: space-evenly;
	}
	.inquiry_bottom2_btn1{
		width: 240rpx;
		height: 72rpx;
		background: #3891ED;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #FFFFFF;
		line-height: 72rpx;
		text-align: center;
	}
	.inquiry_bottom2_btn2{
		width: 240rpx;
		height: 72rpx;
		background: #C80000;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #FFFFFF;
		line-height: 72rpx;
		text-align: center;
	}
</style>