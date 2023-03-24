<template>
	<view class="order">
		<view class="order_top">
			<image class="order_top_img" src="../../static/img/time.png" mode=""></image>
			<view class="order_top_text">
				待确认
			</view>
		</view>
		<view class="order_time">
			<view class="order_time_text1">
				要货时间：2019-04-15 09:00
			</view>
			<view class="order_time_text2">
				配送方式：厂家配送
			</view>
			<view class="order_time_text3">
				<view class="order_time_text3_t1">
					开具发票
				</view>
				<view class="order_time_text3_t2" @click="lookOrder">
					查看发票
				</view>
			</view>
			<view class="order_time_text4">
				备注：无
			</view>
		</view>
		<view class="order_all" v-for="(item,index) in list" :key="index">
			<view class="order_all_yi">
				<view class="order_all_yi_text">
					{{item.text1}}
				</view>
				<image class="order_all_yi_img" :src="item.url1" mode=""></image>
			</view>
			<view class="order_all_er">
				<image class="order_all_er_img" :src="item.url2" mode=""></image>
				<view class="order_all_er_center">
					<view class="order_all_er_center_text1">
						{{item.text2}}
					</view>
					<view class="order_all_er_center_text2">
						{{item.text3}}
					</view>
					<view class="order_all_er_center_text3">
						{{item.text4}}
					</view>
				</view>
				<view class="order_all_er_right">
					{{item.text5}}
				</view>
			</view>
			<view class="order_all_san">
				共1种 合计：100元 数量：100千克
			</view>
		</view>
		<view class="order_details">
			<view class="order_details_yi">
				<view class="order_details_yi_text1">
					订单编号：859875661423
				</view>
				<view class="order_details_yi_text2">
					复制
				</view>
			</view>
			<view class="order_details_er">
				下单时间：2019-04-12 16:19:11
			</view>
			<view class="order_details_er">
				收货地址：北京市朝阳区望京园龙湖冠宇
			</view>
			<view class="order_details_er">
				收货人：王小明 19928888221
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
				取消订单
			</view>
		</view>
		<uni-popup ref="popup" type="bottom">
			<view class="eject">
				<view class="eject_title">
					取消订单
				</view>
				<view class="eject_yi">
					<view class="eject_yi_text">
						我不想买了
					</view>
					<image class="eject_yi_img" src="../../static/img/yuan1.png" mode=""></image>
					<!-- <image class="eject_yi_img" src="../../static/img/yuan2.png" mode=""></image> -->
				</view>
				<view class="eject_yi1">
					<view class="eject_yi_text">
						信息错误, 重新拍
					</view>
					<image class="eject_yi_img" src="../../static/img/yuan1.png" mode=""></image>
					<!-- <image class="eject_yi_img" src="../../static/img/yuan2.png" mode=""></image> -->
				</view>
				<view class="eject_yi1">
					<view class="eject_yi_text">
						卖家缺货
					</view>
					<image class="eject_yi_img" src="../../static/img/yuan1.png" mode=""></image>
					<!-- <image class="eject_yi_img" src="../../static/img/yuan2.png" mode=""></image> -->
				</view>
				<view class="eject_yi1">
					<view class="eject_yi_text">
						其他原因
					</view>
					<image class="eject_yi_img" src="../../static/img/yuan1.png" mode=""></image>
					<!-- <image class="eject_yi_img" src="../../static/img/yuan2.png" mode=""></image> -->
				</view>
				<view class="eject_er">
					<view class="eject_er_no">
						暂不取消
					</view>
					<view class="eject_er_yes">
						确认取消
					</view>
				</view>
			</view>
		</uni-popup>
	</view>
</template>

<script>
	export default{
		data(){
			return{
				list:[
					{
						url1:'../../static/img/shangbiao.png',
						url2:'../../static/img/root2.png',
						url3:'../../static/img/kefu2.png',
						url4:'../../static/img/phone2.png',
						text1:'JD Apple 产品京东自营旗舰店',
						text2:'猪肉-SKU名称',
						text3:'鲜品-中国-国家101厂',
						text4:'单价：￥99.00/千克',
						text5:'数量：100千克',
						text6:'在线咨询',
						text7:'电话沟通',
						text8:'取消订单',
						text9:'查看详情',
					}
				]
			}
		},
		methods:{
			lookOrder(){
				uni.navigateTo({
					url:'/pages/faao/index'
				})
			},
			open(){
			       // 通过组件定义的ref调用uni-popup方法 ,如果传入参数 ，type 属性将失效 ，仅支持 ['top','left','bottom','right','center']
			       this.$refs.popup.open('bottom')
			     }
		}
	}
</script>

<style>
	.order{
		height: 1354rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		position: relative;
	}
	.order_top{
		height: 90rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		display: flex;
		align-items: center;
		padding: 30rpx;
		border-top: 2rpx solid #f8f8f8;
		border-bottom: 2rpx solid #f8f8f8;
	}
	.order_top_img{
		width: 90rpx;
		height: 90rpx;
	}
	.order_top_text{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 38rpx;
		margin-left: 20rpx;
	}
	.order_time{
		height: 220rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		padding: 30rpx;
		margin-bottom: 20rpx;
	}
	.order_time_text1{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
	}
	.order_time_text2{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
		margin-top: 20rpx;
	}
	.order_time_text3{
		display: flex;
		justify-content: space-between;
		margin-top: 20rpx;
	}
	.order_time_text3_t1{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
	}
	.order_time_text3_t2{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #3891ED;
		line-height: 33rpx;
	}
	.order_time_text4{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
		margin-top: 20rpx;
	}
	.order_all{
		height: 312rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		padding: 20rpx 30rpx 30rpx 32rpx;
		margin-bottom: 20rpx;
	}
	.order_all_yi{
		height: 44rpx;
		display: flex;
		align-items: center;
	}
	.order_all_yi_text{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 38rpx;
	}
	.order_all_yi_img{
		width: 36rpx;
		height: 36rpx;
		margin-left: 10rpx;
	}
	.order_all_er{
		display: flex;
		height: 178rpx;
		margin-top: 30rpx;
		border-bottom: 2rpx solid #f8f8f8;
	}
	.order_all_er_img{
		width: 148rpx;
		height: 148rpx;
	}
	.order_all_er_center{
		margin-left: 20rpx;
		height: 148rpx;
	}
	.order_all_er_center_text1{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 38rpx;
	}
	.order_all_er_center_text2{
		height: 34rpx;
		font-size: 24rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #666666;
		line-height: 28rpx;
		margin-top: 8rpx;
		margin-bottom: 12rpx;
	}
	.order_all_er_center_text3{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #C80000;
		line-height: 33rpx;
	}
	.order_all_er_right{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
		margin-left: 64rpx;
		margin-top: 100rpx;
	}
	.order_all_san{
		height: 80rpx;
		line-height: 80rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		margin-left: 234rpx;
	}
	.order_details{
		height: 220rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		padding: 30rpx;
	}
	.order_details_yi{
		display: flex;
	}
	.order_details_yi_text1{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 40rpx;
	}
	.order_details_yi_text2{
		width: 80rpx;
		height: 40rpx;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		border: 2rpx solid #3891ED;
		font-size: 24rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #3891ED;
		line-height: 40rpx;
		text-align: center;
		margin-left: 26rpx;
	}
	.order_details_er{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
		margin-top: 20rpx;
	}
	.order_bottom{
		position: absolute;
		bottom: 0;
		width: 100%;
		height: 104rpx;
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
		height: 34rpx;
		font-size: 24rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 28rpx;
		margin-left: 10rpx;
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
		margin-left: 36rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #3891ED;
		line-height: 60rpx;
		text-align: center;
		margin-left: 178rpx;
	}
	.eject{
		height: 658rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
	}
	.eject_title{
		width: 100%;
		text-align: center;
		padding-top: 42rpx;
		height: 58rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 58rpx;
	}
	.eject_yi{
		margin: 30rpx 40rpx 0 42rpx;
		display: flex;
		height: 58rpx;
		align-items: center;
		justify-content: space-between;
	}
	.eject_yi_text{
		height: 58rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 58rpx;
	}
	.eject_yi_img{
		width: 56rpx;
		height: 56rpx;
	}
	.eject_yi1{
		margin-top: 20rpx;
		margin-left: 42rpx;
		margin-right: 40rpx;
		display: flex;
		height: 58rpx;
		align-items: center;
		justify-content: space-between;
	}
	.eject_er{
		margin: 130rpx 30rpx 60rpx 30rpx;
		height: 88rpx;
		display: flex;
		align-items: center;
	}
	.eject_er_no{
		width: 330rpx;
		height: 88rpx;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		border: 2rpx solid #333333;
		line-height: 88rpx;
		text-align: center;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
	}
	.eject_er_yes{
		width: 330rpx;
		height: 88rpx;
		background: #3891ED;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		line-height: 88rpx;
		text-align: center;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #FFFFFF;
		margin-left: 30rpx;
	}
</style>