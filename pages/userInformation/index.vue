<template>
	<view class="information">
		<view class="information_top">
			<view class="information_top_sculpture">
				头像
			</view>
			<view class="information_top_right">
				<image class="information_top_right_img1" src="../../static/img/touxiang.png" mode=""></image>
				<image class="information_top_right_img2" src="../../static/img/you.png" mode=""></image>
			</view>
		</view>
		<view class="information_top">
			<view class="information_top_sculpture">
				昵称
			</view>
			<view class="information_top_right">
				<view class="information_top_right_text">
					我
				</view>
				<image class="information_top_right_img2" src="../../static/img/you.png" mode=""></image>
			</view>
		</view>
		<view class="information_top" @click="gender">
			<view class="information_top_sculpture">
				性别
			</view>
			<view class="information_top_right">
				<view class="information_top_right_text">
					男
				</view>
				<image class="information_top_right_img2" src="../../static/img/you.png" mode=""></image>
			</view>
		</view>
		<u-picker :show="show" title="请选择性别" @confirm="define" @cancel="close" :columns="columns"></u-picker>
		<view class="information_top" @click="gender">
			<view class="information_top_sculpture">
				生日
			</view>
			<view class="information_top_right">
				<view class="information_top_right_text">
					1996.11.02
				</view>
				<image class="information_top_right_img2" src="../../static/img/you.png" mode=""></image>
			</view>
		</view>
		<u-picker :show="show" title="选择生日" @confirm="define" @cancel="close" :columns="columnsB"></u-picker>
		<view class="information_top">
			<view class="information_top_sculpture">
				采购品类
			</view>
			<view class="information_top_right">
				<view class="information_top_right_text">
					请选择
				</view>
				<image class="information_top_right_img2" src="../../static/img/you.png" mode=""></image>
			</view>
		</view>
		<view class="information_top" @click="gender">
			<view class="information_top_sculpture">
				所属地区
			</view>
			<view class="information_top_right">
				<view class="information_top_right_text">
					请选择
				</view>
				<image class="information_top_right_img2" src="../../static/img/you.png" mode=""></image>
			</view>
		</view>
		<u-picker :show="show" title="选择地区" @confirm="define" @cancel="close" :columns="columnsAddress"></u-picker>
		<view class="information_top">
			<view class="information_top_sculpture">
				详细地址
			</view>
			<view class="information_top_right">
				<view class="information_top_right_text">
					请输入
				</view>
				<image class="information_top_right_img2" src="../../static/img/you.png" mode=""></image>
			</view>
		</view>
	</view>
</template>

<script>
	export default{
		data(){
			return{
				show:false,
				columns: [
					['男', '女']
				        ],
				columnsB:[
					['2000', '2001','2002','2003','2004','2005','2006','2007'],
					['1月', '2月', '3月', '4月','5月','6月','7月', '8月', '9月', '10月','11月','12月'],
					[
						'1日', '2日', '3日', '4日','5日','6日','7日', '8日', '9日', '10日',
						'11日', '12日', '13日', '14日','15日','16日','17日', '18日', '19日', '20日',
						'21日', '22日', '23日', '24日','25日','26日','27日', '28日', '29日', '30日',
						'31日',
					],
				],
				columnsAddress:[
					['中国', '美国'],
					['深圳', '厦门', '上海', '拉萨']
				],
			}
		},
		methods:{
			gender(){
				this.show =! this.show
			},
			close(){
				this.show = false
			},
			define(e){
				console.log('confirm', e.value,e)
				this.show = false
			}
		}
	}
</script>

<style>
	.information{
		height: 1624rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.information_top{
		height: 104rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		display: flex;
		align-items: center;
		justify-content: space-between;
		padding: 0 40rpx 0 38rpx;
		border-top: 2rpx solid #f8f8f8;
	}
	.information_top_sculpture{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 38rpx;
	}
	.information_top_right{
		display: flex;
		align-items: center;
	}
	.information_top_right_img1{
		width: 60rpx;
		height: 60rpx;
	}
	.information_top_right_img2{
		width: 48rpx;
		height: 48rpx;
		margin-left: 4rpx;
		margin-bottom: 6rpx;
	}
	.information_top_right_text{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
	}
</style>