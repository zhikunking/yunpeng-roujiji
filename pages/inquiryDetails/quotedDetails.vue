<template>
	<view class="inquiry">
		<view class="inquiry_top">
			<view class="inquiry_top_left">
				已报价
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
				<view class="inquiry_supplier_no_btn1">
					<view class="inquiry_supplier_no_btn1_t1">
						20
					</view>
					<view class="inquiry_supplier_no_btn1_t2">
						待选商
					</view>
				</view>
				<view class="inquiry_supplier_no_btn1">
					<view class="inquiry_supplier_no_btn1_t1">
						10
					</view>
					<view class="inquiry_supplier_no_btn1_t2">
						已成交
					</view>
				</view>
			</view>
		</view>
		<view class="inquiry_selected">
			<view class="inquiry_selected_top">
				<view class="inquiry_selected_top_text">
					待选商
				</view>
				<view class="inquiry_selected_top_select">
					<view class="inquiry_selected_top_select1">
						<view class="inquiry_selected_top_select_text">
							价格优先
						</view>
						<image class="inquiry_selected_top_select_img" src="../../static/img/xia1.png" mode=""></image>
					</view>
					<view class="inquiry_selected_top_select_up">
						收起
					</view>
				</view>
			</view>
			<view class="inquiry_selected_enterprise">
				<view class="inquiry_selected_bossName">
					山东肉集集信息科技有限责任公司（企业）
				</view>
				<view class="inquiry_selected_bossTime">
					报价时间：2022年12月12日 11:00
				</view>
			</view>
			<view class="inquiry_selected_information">
				<view class="inquiry_selected_information_text1">
					鸡翅 冻品 50千克
				</view>
				<view class="inquiry_selected_information_text2">
					<view class="inquiry_selected_information_text2_left">
						国家长号：工厂101
					</view>
					<view class="inquiry_selected_information_text2_right">
						生产日期：2022年4月
					</view>
				</view>
				<view class="inquiry_selected_information_text2">
					<view class="inquiry_selected_information_text2_left">
						可供数量：10千克
					</view>
					<view class="inquiry_selected_information_text2_right">
						单位：100元/千克
					</view>
				</view>
				<view class="inquiry_selected_information_text2">
					<view class="inquiry_selected_information_text2_left">
						发货地：北京市北京城区丰台区
					</view>
					<view class="inquiry_selected_information_text2_right1">
						距离<text class="inquiry_selected_information_text2_right1_bai">100</text>公里
					</view>
				</view>
			</view>
			<view class="order_bottom">
				<image class="order_all_san_img" src="../../static/img/kefu2.png" mode=""></image>
				<view class="order_all_san_text">
					在线咨询
				</view>
				<image class="order_all_san_img1" src="../../static/img/phone2.png" mode=""></image>
				<view class="order_all_san_text">
					电话沟通
				</view>
				<view class="order_all_san_btn1" @click="open">
					立即下单
				</view>
			</view>
		</view>
		<IndexActive2 />
		<view class="inquiry_bottom2">
			<view class="inquiry_bottom2_btn2">
				停止询价
			</view>
		</view>
	</view>
</template>

<script>
	import IndexActive from "@/pages/inquiryDetails/index-active"
	import IndexActive2 from "@/pages/inquiryDetails/index-active2"
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
		height: 3790rpx;
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
		color: #3891ED;
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
		height: 390rpx;
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
		width: 690rpx;
		height: 148rpx;
		background: #F5F5F5;
		border-radius: 20rpx 20rpx 20rpx 20rpx;
		opacity: 1;
		margin: 30rpx;
		display: flex;
		justify-content: space-evenly;
		align-items: center;
	}
	.inquiry_supplier_no_btn1{
		text-align: center;
	}
	.inquiry_supplier_no_btn1_t1{
		height: 50rpx;
		font-size: 36rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 42rpx;
	}
	.inquiry_supplier_no_btn1_t2{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
	}
	.inquiry_selected{
		height: 540rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		margin-bottom: 20rpx;
		padding: 30rpx 30rpx 20rpx 30rpx;
	}
	.inquiry_selected_top{
		height: 76rpx;
		display: flex;
		border-bottom: 2rpx solid #f7f7f7;
		justify-content: space-between;
	}
	.inquiry_selected_top_text{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 38rpx;
	}
	.inquiry_selected_top_select{
		display: flex;
	}
	.inquiry_selected_top_select1{
		width: 182rpx;
		height: 48rpx;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		border: 2rpx solid #C1C1C1;
		display: flex;
	}
	.inquiry_selected_top_select_text{
		width: 112rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		margin-left: 20rpx;
	}
	.inquiry_selected_top_select_img{
		width: 32rpx;
		height: 32rpx;
		margin-top: 6rpx;
	}
	.inquiry_selected_top_select_up{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #3891ED;
		line-height: 33rpx;
		margin-left: 20rpx;
		margin-top: 8rpx;
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
		justify-content: center;
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
	.inquiry_selected_enterprise{
		height: 104rpx;
		margin-top: 30rpx;
		border-bottom: 2rpx solid #f7f7f7;
	}
	.inquiry_selected_bossName{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #C80000;
		line-height: 33rpx;
	}
	.inquiry_selected_bossTime{
		height: 34rpx;
		font-size: 24rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #666666;
		line-height: 28rpx;
		margin-top: 10rpx;
	}
	.inquiry_selected_information{
		height: 220rpx;
		margin-top: 30rpx;
		border-bottom: 2rpx solid #f7f7f7;
	}
	.inquiry_selected_information_text1{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
	}
	.inquiry_selected_information_text2{
		display: flex;
		height: 40rpx;
		margin-top: 10rpx;
	}
	.inquiry_selected_information_text2_left{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
	}
	.inquiry_selected_information_text2_right{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
		margin-left: 124rpx;
	}
	.inquiry_selected_information_text2_right1{
		margin-left: 124rpx;
		height: 34rpx;
		font-size: 24rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #666666;
		line-height: 28rpx;
	}
	.inquiry_selected_information_text2_right1_bai{
		color: #3891ED;
	}
	.order_bottom{
		height: 94rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		display: flex;
		align-items: center;
		padding: 0 30rpx;
	}
	.order_all_san_img{
		width: 36rpx;
		height: 36rpx;
	}
	.order_all_san_text{
		width: 122rpx;
		height: 34rpx;
		font-size: 24rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 28rpx;
		margin-left: 20rpx;
	}
	.order_all_san_img1{
		width: 36rpx;
		height: 36rpx;
		margin-left: 30rpx;
	}
	.order_all_san_btn1{
		width: 160rpx;
		height: 60rpx;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		border: 2rpx solid #3891ED;
		background: #3891ED;
		margin-left: 36rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #FFFFFF;
		line-height: 60rpx;
		text-align: center;
		margin-left: 128rpx;
	}
</style>