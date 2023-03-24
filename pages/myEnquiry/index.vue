<template>
	<view class="enquiry">
		<view class="enquiry_nav">
			<uni-segmented-control :current="current" :values="tabs" @clickItem="onClickItem" styleType="text"></uni-segmented-control>
		</view>
		<view class="enquiry_all" v-for="(item,index) in list" :key="index">
			<view class="enquiry_all_yi">
				<view class="enquiry_all_yi_text1">
					{{item.text1}}
				</view>
				<view class="enquiry_all_yi_text2" v-if="index == 0">待报价</view>
				<view class="enquiry_all_yi_text3" v-if="index == 1">已报价</view>
				<view class="enquiry_all_yi_text4" v-if="index == 2">已结束</view>
			</view>
			<view class="enquiry_all_er">
				{{item.text2}}
			</view>
			<view class="enquiry_all_er">
				{{item.text3}}
			</view>
			<view class="enquiry_all_er">
				{{item.text4}}
			</view>
			<view class="enquiry_all_san">
				<view class="enquiry_all_san_t1">
					<view class="enquiry_all_san_t1_text1">
						{{item.text7}}
					</view>
					<view class="enquiry_all_san_t1_text2">
						{{item.text5}}
					</view>
				</view>
				<view class="enquiry_all_san_t2">
					<view class="enquiry_all_san_t2_text1">
						{{item.text6}}
					</view>
					<view class="enquiry_all_san_t2_text2">
						{{item.text8}}
					</view>
				</view>
				<view class="enquiry_all_san_t3">
					<image class="enquiry_all_san_img" src="../../static/img/you.png" mode=""></image>
				</view>
			</view>
			<view class="enquiry_all_si">
				<view class="enquiry_all_si_btn1">
					暂停询价
				</view>
				<view class="enquiry_all_si_btn2">
					修改询价单
				</view>
			</view>
		</view>
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
						text1:'猪肉100千克 | 现货',
						text2:'鸡胸肉 冻品 50千克/鸡翅 冻品 50千克',
						text3:'生产国家：不限',
						text4:'要货时间：2022年11月20日前',
						text5:'待选商',
						text6:'10',
						text7:'20',
						text8:'已成交'
					},
					{
						text1:'猪肉100千克 | 现货',
						text2:'鸡胸肉 冻品 50千克/鸡翅 冻品 50千克',
						text3:'生产国家：不限',
						text4:'要货时间：2022年11月20日前',
						text5:'待选商',
						text6:'10',
						text7:'20',
						text8:'已成交'
					},
					{
						text1:'猪肉100千克 | 现货',
						text2:'鸡胸肉 冻品 50千克/鸡翅 冻品 50千克',
						text3:'生产国家：不限',
						text4:'要货时间：2022年11月20日前',
						text5:'待选商',
						text6:'10',
						text7:'20',
						text8:'已成交'
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
		}
	}
</script>

<style>
	.enquiry{
		height: 1822rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.enquiry_nav{
		height: 88rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		border-bottom: 2rpx solid #F8F8F8;
	}
	.enquiry_all{
		height: 462rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		padding: 20rpx 30rpx 30rpx 30rpx;
		margin-bottom: 20rpx;
	}
	.enquiry_all_yi{
		display: flex;
		justify-content: space-between;
	}
	.enquiry_all_yi_text1{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 38rpx;
	}
	.enquiry_all_yi_text2{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #EB3F4A;
		line-height: 33rpx;
	}
	.enquiry_all_yi_text3{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #3891ED;
		line-height: 33rpx;
	}
	.enquiry_all_yi_text4{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
		line-height: 33rpx;
	}
	.enquiry_all_er{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #666666;
		line-height: 33rpx;
		margin-top: 20rpx;
	}
	.enquiry_all_san{
		width: 690rpx;
		height: 148rpx;
		background: #F5F5F5;
		border-radius: 20rpx 20rpx 20rpx 20rpx;
		opacity: 1;
		margin-top: 20rpx;
		display: flex;
		align-items: center;
	}
	.enquiry_all_san_t1{
		width: 180rpx;
		margin-left: 130rpx;
		text-align: center;
	}
	.enquiry_all_san_t2{
		margin-left: 120rpx;
		text-align: center;
	}
	.enquiry_all_san_img{
		width: 48rpx;
		height: 48rpx;
		margin-left: 98rpx;
	}
	.enquiry_all_si{
		display: flex;
		margin-top: 20rpx;
		margin-left: 352rpx;
	}
	.enquiry_all_si_btn1{
		width: 160rpx;
		height: 60rpx;
		line-height: 60rpx;
		text-align: center;
		background: #C80000;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #FFFFFF;
	}
	.enquiry_all_si_btn2{
		width: 188rpx;
		height: 60rpx;
		line-height: 60rpx;
		text-align: center;
		background: #3891ED;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #FFFFFF;
		margin-left: 20rpx;
	}
</style>