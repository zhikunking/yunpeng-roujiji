<template>
	<view class="order">
		<view class="order_nav">
			<uni-segmented-control :current="current" :values="tabs" @clickItem="onClickItem" styleType="text"></uni-segmented-control>
		</view>
		<view class="order_all" v-for="(item,index) in list" :key="index">
			<view class="order_all_yi">
				<view class="order_all_yi_text">
					{{item.text1}}
				</view>
				<image class="order_all_yi_img" :src="item.url1" mode=""></image>
				<view class="order_all_yi_text1" v-if="index == 0">待确认</view>
				<view class="order_all_yi_text2" v-if="index == 1">已确认</view>
				<view class="order_all_yi_text3" v-if="index == 2">已失效</view>
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
				<image class="order_all_san_img" :src="item.url3" mode=""></image>
				<view class="order_all_san_text">
					{{item.text6}}
				</view>
				<image class="order_all_san_img1" :src="item.url4" mode=""></image>
				<view class="order_all_san_text">
					{{item.text7}}
				</view>
				<view class="order_all_san_btn1" @click="open">
					{{item.text8}}
				</view>
				<view class="order_all_san_btn2">
					{{item.text9}}
				</view>
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
				current: 0,
				status:0,
				activeIndex:'',
				tabs:['全部','待确认','已确认','已失效'],
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
					},
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
					},
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
					},
				]
			}
		},
		methods:{
			onClickItem(e){
				console.log(e)
				 if (this.current != e.currentIndex) {
				        this.current = e.currentIndex;
				      }
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
		height: 1624rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.order_nav{
		height: 88rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		border-bottom: 2rpx solid #F8F8F8;
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
	.order_all_yi_text1{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #EB3F4A;
		line-height: 33rpx;
		margin-left: 122rpx;
	}
	.order_all_yi_text2{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #3891ED;
		line-height: 33rpx;
		margin-left: 122rpx;
	}
	.order_all_yi_text3{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
		line-height: 33rpx;
		margin-left: 122rpx;
	}
	.order_all_er{
		display: flex;
		height: 148rpx;
		margin-top: 30rpx;
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
		height: 60rpx;
		margin-top: 40rpx;
		display: flex;
		align-items: center;
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
		border: 2rpx solid #999999;
		margin-left: 36rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 60rpx;
		text-align: center;
	}
	.order_all_san_btn2{
		width: 160rpx;
		height: 60rpx;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		border: 2rpx solid #999999;
		margin-left: 10rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 60rpx;
		text-align: center;
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