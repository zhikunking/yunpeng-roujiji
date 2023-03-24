<template>
	<view class="my">
		<view class="my_top">
			<view class="my_top_status">
				<image class="my_top_status-img" src="../../static/img/my1.png" mode=""></image>
				<view class="my_top_status-text">切换到商家端</view>
			</view>
			<view class="my_top_img">
				<image class="my_top_img-t1" src="../../static/img/my2.png" mode=""></image>
				<view class="my_top_img-t2">
					<view class="my_top_img-t2-text1">
						高质量人类
						<image class="my_top_img-t3-img1" src="../../static/img/geren2.png" mode=""></image>
						<image class="my_top_img-t3-img2" src="../../static/img/geti2.png" mode=""></image>
						<image class="my_top_img-t3-img2" src="../../static/img/qiye2.png" mode=""></image>
					</view>
					<view class="my_top_img-t2-text2">
						登录手机号：10028882221
					</view>
				</view>
			</view>
		</view>
		<view class="my_top_attestation">
			完成认证，才可参与交易<text class="my_top_attestation-text">去认证</text>
		</view>
		<view class="my_top_collect">
			<image class="my_top_collect_img1" src="../../static/img/my3.png" mode=""></image>
			<view class="my_top_collect_text1">商品收藏22</view>
			<image class="my_top_collect_img2" src="../../static/img/my4.png" mode=""></image>
			<view class="my_top_collect_text2">我的供应商25</view>
			<image class="my_top_collect_img2" src="../../static/img/my5.png" mode=""></image>
			<view class="my_top_collect_text2">我的足迹90</view>
		</view>
		<view class="my_goods">
			<view class="my_goods_order">
				<view class="my_goods_order-left">
					我的订单
				</view>
				<view class="my_goods_order_right">
					<view class="my_goods_order_right_text">
						全部订单
					</view>
					<image class="my_goods_order_right_img" src="../../static/img/you.png" mode=""></image>
				</view>
			</view>
			<view class="my_goods_img">
				<view class="my_goods_img_queren">
					<image class="my_goods_img_queren_image" src="../../static/img/my7.png" mode=""></image>
					<view class="my_goods_img_queren_text2">
						1
					</view>
					<view class="my_goods_img_queren_text">
						待确认
					</view>
				</view>
				<view class="my_goods_img_queren">
					<image class="my_goods_img_queren_image" src="../../static/img/my8.png" mode=""></image>
					<view class="my_goods_img_queren_text">
						已确认
					</view>
				</view>
			</view>
		</view>
		<view class="my_enquiry">
			<view class="my_goods_order">
				<view class="my_goods_order-left">
					我的询价单
				</view>
				<view class="my_goods_order_right">
					<view class="my_goods_order_right_text">
						全部询价单
					</view>
					<image class="my_goods_order_right_img" src="../../static/img/you.png" mode=""></image>
				</view>
			</view>
			<view class="my_enquiry_order">
				<view class="my_enquiry_order_noEnquiry">
					<view class="my_enquiry_order_noEnquiry_yi">
						20
					</view>
					<view class="my_enquiry_order_noEnquiry_er">
						待报价
					</view>
				</view>
				<view class="my_enquiry_order_noEnquiry">
					<view class="my_enquiry_order_noEnquiry_yi">
						10
					</view>
					<view class="my_enquiry_order_noEnquiry_er">
						待选商
					</view>
				</view>
				<view class="my_enquiry_order_noEnquiry">
					<view class="my_enquiry_order_noEnquiry_yi">
						0
					</view>
					<view class="my_enquiry_order_noEnquiry_er">
						已成交
					</view>
				</view>
			</view>
			<view class="my_enquiry_bottom">
				<view class="my_enquiry_bottom_text">
					常用功能
				</view>
				<view class="my_enquiry_bottom_list">
					<view class="my_enquiry_bottom_list_t1">
						<image class="my_enquiry_bottom_list_img" src="../../static/img/my9.png" mode=""></image>
						<view class="my_enquiry_bottom_list_text">
							渠道合伙人
						</view>
					</view>
					<view class="my_enquiry_bottom_list_t2">
						<image class="my_enquiry_bottom_list_img" src="../../static/img/my10.png" mode=""></image>
						<view class="my_enquiry_bottom_list_text">
							地址管理
						</view>
					</view>
					<view class="my_enquiry_bottom_list_t2">
						<image class="my_enquiry_bottom_list_img" src="../../static/img/my11.png" mode=""></image>
						<view class="my_enquiry_bottom_list_text">
							客户服务
						</view>
					</view>
					<view class="my_enquiry_bottom_list_t2">
						<image class="my_enquiry_bottom_list_img" src="../../static/img/my12.png" mode=""></image>
						<view class="my_enquiry_bottom_list_text">
							商家入驻
						</view>
					</view>
					<view class="my_enquiry_bottom_list_t1">
						<image class="my_enquiry_bottom_list_img" src="../../static/img/my13.png" mode=""></image>
						<view class="my_enquiry_bottom_list_text">
							意见反馈
						</view>
					</view>
					<view class="my_enquiry_bottom_list_t3">
						<image class="my_enquiry_bottom_list_img" src="../../static/img/my14.png" mode=""></image>
						<view class="my_enquiry_bottom_list_text">
							认证管理
						</view>
					</view>
					<view class="my_enquiry_bottom_list_t4">
						<image class="my_enquiry_bottom_list_img" src="../../static/img/my15.png" mode=""></image>
						<view class="my_enquiry_bottom_list_text">
							设置
						</view>
					</view>
				</view>
					
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
	.my{
		height: 1640rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.my_top{
		height: 294rpx;
		background: #3891ED;
	}
	.my_top_status{
		width: 246rpx;
		height: 60rpx;
		background: #FFFFFF;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 0.3;
		margin-left: 30rpx;
		display: flex;
		align-items: center;
	}
	.my_top_status-img{
		width: 27rpx;
		height: 15rpx;
		margin-left: 20rpx;
	}
	.my_top_status-text{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #FFFFFF;
		line-height: 33rpx;
		margin-left: 2rpx;
	}
	.my_top_img{
		height: 136rpx;
		display: flex;
		align-items: center;
	}
	.my_top_img-t1{
		width: 136rpx;
		height: 136rpx;
		margin-top: 84rpx;
		margin-left: 42rpx;
	}
	.my_top_img-t2{
		margin-left: 20rpx;
	}
	.my_top_img-t2-text1{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #FFFFFF;
		line-height: 38rpx;
		margin-top: 60rpx;
	}
	.my_top_img-t2-text2{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #FFFFFF;
		line-height: 33rpx;
		margin-top: 20rpx;
	}
	.my_top_img-t3{
		display: flex;
	}
	.my_top_img-t3-img1{
		width: 92rpx;
		height: 50rpx;
		margin-left: 62rpx;
	}
	.my_top_img-t3-img2{
		width: 92rpx;
		height: 50rpx;
		margin-left: 12rpx;
	}
	.my_top_attestation{
		width: 688rpx;
		height: 104rpx;
		background: #FFFFFF;
		border-radius: 12rpx 12rpx 12rpx 12rpx;
		opacity: 1;
		margin: 20rpx 32rpx 20rpx 30rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 104rpx;
		text-align: center;
	}
	.my_top_attestation-text{
		color: #3891ED;
	}
	.my_top_collect{
		width: 688rpx;
		height: 104rpx;
		background: #FFFFFF;
		border-radius: 12rpx 12rpx 12rpx 12rpx;
		opacity: 1;
		margin: 20rpx 32rpx 20rpx 30rpx;
		display: flex;
		align-items: center;
	}
	.my_top_collect_img1{
		width: 40rpx;
		height: 40rpx;
		margin-left: 20rpx;
	}
	.my_top_collect_text1{
		margin-left: 4rpx;
		height: 36rpx;
		font-size: 26rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 30rpx;
	}
	.my_top_collect_img2{
		width: 40rpx;
		height: 40rpx;
		margin-left: 42rpx;
	}
	.my_top_collect_text2{
		margin-left: 4rpx;
		height: 36rpx;
		font-size: 26rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 30rpx;
	}
	.my_goods{
		width: 690rpx;
		height: 246rpx;
		background: #FFFFFF;
		border-radius: 12rpx 12rpx 12rpx 12rpx;
		opacity: 1;
		margin: 20rpx 30rpx;
	}
	.my_goods_order{
		display: flex;
		align-items: center;
		justify-content: space-between;
		padding-top: 32rpx;
		margin-left: 30rpx;
		margin-bottom: 20rpx;
	}
	.my_goods_order-left{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
	}
	.my_goods_order_right{
		display: flex;
	}
	.my_goods_order_right_text{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
		margin-top: 2rpx;
	}
	.my_goods_order_right_img{
		width: 40rpx;
		height: 40rpx;
	}
	.my_goods_img{
		height: 174rpx;
		display: flex;
		/* align-items: center; */
	}
	.my_goods_img_queren{
		width: 232rpx;
		text-align: center;
		position: relative;
	}
	.my_goods_img_queren_image{
		width: 64rpx;
		height: 64rpx;
		/* margin-left: 84rpx; */
	}
	.my_goods_img_queren_text{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
		margin-top: 20rpx;
	}
	.my_goods_img_queren_text2{
		width: 24rpx;
		height: 24rpx;
		background: #DF0202;
		opacity: 1;
		border-radius: 50%;
		font-size: 20rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #FFFFFF;
		text-align: center;
		line-height: 24rpx;
		position: absolute;
		top: 0;
		right: 34%;
	}
	.my_enquiry{
		width: 690rpx;
		height: 220rpx;
		background: #FFFFFF;
		border-radius: 12rpx 12rpx 12rpx 12rpx;
		opacity: 1;
		margin-left: 30rpx;
	}
	.my_enquiry_order{
		height: 162rpx;
		display: flex;
		/* align-items: center; */
		justify-content: space-evenly;
	}
	.my_enquiry_order_noEnquiry{
		height: 162rpx;
		text-align: center;
	}
	.my_enquiry_order_noEnquiry_yi{
		width: 44rpx;
		height: 50rpx;
		font-size: 36rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 42rpx;
		margin-left: 18rpx;
	}
	.my_enquiry_order_noEnquiry_er{
		width: 84rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
	}
	.my_enquiry_bottom{
		width: 690rpx;
		height: 380rpx;
		background: #FFFFFF;
		border-radius: 12rpx 12rpx 12rpx 12rpx;
		opacity: 1;
	}
	.my_enquiry_bottom_text{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
		padding-top: 32rpx;
		margin-left: 16rpx;
	}
	.my_enquiry_bottom_list{
		height: 164rpx;
		margin-left: 34rpx;
		margin-right: 30rpx;
		margin-top: 20rpx;
		display: flex;
		flex-wrap: wrap;
	}
	.my_enquiry_bottom_list_t1{
		text-align: center;
		margin-bottom: 20rpx;
	}
	.my_enquiry_bottom_list_t2{
		text-align: center;
		margin-left: 46rpx;
		margin-bottom: 20rpx;
	}
	.my_enquiry_bottom_list_t3{
		text-align: center;
		margin-left: 76rpx;
		margin-bottom: 20rpx;
	}
	.my_enquiry_bottom_list_t4{
		text-align: center;
		margin-left: 66rpx;
		margin-bottom: 20rpx;
	}
	.my_enquiry_bottom_list_img{
		width: 64rpx;
		height: 64rpx;
	}
	.my_enquiry_bottom_list_text{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
	}
</style>