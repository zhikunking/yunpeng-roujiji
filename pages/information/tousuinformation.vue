<template>
	<view class="tousu-information">
		<view class="tousu-information-top">
			<view class="tousu-information-top-text1">
				投诉人
			</view>
			<view class="tousu-information-top-text2">
				<image class="tousu-information-top-text2-t1" src="../../static/img/tupian.png" mode=""></image>
				<view class="tousu-information-top-text2-t2">
					黑龙江哈尔滨食品有限公司
				</view>
			</view>
		</view>
		<view class="tousu-information-one">
			<view class="tousu-information-one-text1">详情</view>
			<view class="tousu-information-one-text2"><u-line></u-line></view>
			<view class="tousu-information-one-text3">投诉对象：公司名称</view>
			<view class="tousu-information-one-text3">投诉类型：诈骗</view>
			<view class="tousu-information-one-text3">投诉时间：2020.2.2 12:00</view>
		</view>
		<view class="tousu-information-two">
			<view class="tousu-information-two-text1">投诉标题：无良商家骗钱</view>
			<view class="tousu-information-one-text2"><u-line></u-line></view>
			<view class="tousu-information-one-text3">投诉描述</view>
			<view class="tousu-information-two-text3">iPhone 12高度：146.7毫米；宽度：71.5毫米；厚度：7.4毫米；重量：162克（5.73盎司） [5]  。iPhone 12设计采用了离子玻璃，以及7000系列铝金属外壳。iPhone 12采用了直面边框设计，背部颜色有：黑色、白色、红色、绿色、蓝色、紫色 [2]  。</view>
			<view class="tousu-information-img">
					<image  v-for="(item,index) in list" :key="index" class="tousu-information-two-text4-image" :src="item.url"></image>
			</view>
		</view>
		<view class="tousu-information-three">
			<view class="tousu-information-three-text">留言</view>
			<view class="tousu-information-three-input">
				<image class="tousu-information-three-img" src="../../static/img/edit.png" mode=""></image>
				<input class="tousu-information-three-input2" type="text" placeholder="我来说两句...">
			</view>
				<view class="tousu-information-three-pl-yi">
					<image class="tousu-information-three-pl-yi-img" src="../../static/img/tupian2.png" mode=""></image>
					<view class="tousu-information-three-pl-yi-text">@我的人</view>
					<view class="tousu-information-three-pl-yi-sz">148</view>
					<image class="tousu-information-three-pl-yi-img2" src="../../static/img/zan.png" mode=""></image>
				</view>
				<view class="tousu-information-three-pl-er">
					学习原型设计是我做大的爱好，一份高质量的原型设计稿，能够极大提升沟通效率与沟通质量。
				</view>
				<view class="tousu-information-three-pl-san">
					<view class="tousu-information-three-pl-san-text1">14分钟前·</view>
					<view class="tousu-information-three-pl-san-text2">回复TA</view>
					<image class="tousu-information-three-pl-san-img" src="../../static/img/shenglvehao.png" mode=""></image>
				</view>
				<view class="tousu-information-three-pl-si">
					<view class="tousu-information-three-pl-si-text">
						学习原型设计是我做大的爱好，一份高质量的原型设计稿，能够极大提升沟通效率与沟通质量。
					</view>
					<view class="tousu-information-three-pl-si-text2">
						<view class="tousu-information-three-pl-si-text2-t1">
							查看全部5条回复
						</view>
						<image class="tousu-information-three-pl-si-text2-img" src="../../static/img/right2.png" mode=""></image>
					</view>
				</view>
				<view class="tousu-information-one-text2"><u-line></u-line></view>
				<view class="tousu-information-three-pl-wu">
					<view class="tousu-information-three-pl-wu-text">
						查看全部评价
					</view>
					<image class="tousu-information-three-pl-wu-img" src="../../static/img/you.png" mode=""></image>
				</view>
		</view>
	</view>
</template>

<script>
	export default{
			data(){
				return{
					list:[
						{url:'../../static/img/root2.png'},
						{url:'../../static/img/root2.png'},
						{url:'../../static/img/root2.png'},
						{url:'../../static/img/root2.png'},
						{url:'../../static/img/root2.png'},
						{url:'../../static/img/root2.png'},
						{url:'../../static/img/root2.png'},
						{url:'../../static/img/root2.png'},
						{url:'../../static/img/root2.png'},
						{url:'../../static/img/root2.png'},
						{url:'../../static/img/root2.png'},
						{url:'../../static/img/root2.png'}
					]
				}
		}
	}
</script>

<style>
	.tousu-information{
		height: 3298rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.tousu-information-top{
		height: 206rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
	}
	.tousu-information-top-text1{
		margin-top: 30rpx;
		margin-left: 40rpx;
		width: 96rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 38rpx;
	}
	.tousu-information-top-text2{
		display: flex;
		align-items: center;
		margin-left: 40rpx;
		margin-top: 20rpx;
	}
	.tousu-information-top-text2-t1{
		width: 112rpx;
		height: 112rpx;
	}
	.tousu-information-top-text2-t2{
		width: 384rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 38rpx;
		margin-left: 20rpx;
	}
	.tousu-information-one{
		margin-top: 20rpx;
		height: 314rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
	}
	.tousu-information-one-text1{
			width: 64rpx;
			height: 14rpx;
			font-size: 32rpx;
			font-family: PingFang SC-Bold, PingFang SC;
			font-weight: bold;
			color: #333333;
			line-height: 38rpx;
			padding-top: 30rpx;
			margin-left: 30rpx;
	}
	.tousu-information-one-text2{
		margin: 50rpx 30rpx 20rpx 30rpx;
	}
	.tousu-information-one-text3{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
		margin-bottom: 20rpx;
		margin-left: 30rpx;
	}
	.tousu-information-two{
		margin-top: 40rpx;
		height: 1300rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
	}
	.tousu-information-two-text1{
		width: 352rpx;
		height: 14rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 38rpx;
		padding-top: 30rpx;
		margin-left: 30rpx;
	}
	.tousu-information-two-text3{
		height: 208rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 40rpx;
		margin-bottom: 20rpx;
		margin-left: 30rpx;
	}
	.tousu-information-img{
		width: 728rpx;
		display: flex;
		flex-wrap: wrap;
		margin-left: 10rpx;
		margin-top: 20rpx;
	}
	.tousu-information-two-text4-image{
		margin-left: 22rpx;
		width: 216rpx;
		height: 216rpx;
	}
	.tousu-information-three{
		margin-top: 20rpx;
		width: 100%;
		height: 814rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
	}
	.tousu-information-three-text{
		padding-top: 30rpx;
		margin-left: 30rpx;
		width: 168rpx;
		height: 58rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 58rpx;
	}
	.tousu-information-three-input{
		width: 690rpx;
		height: 80rpx;
		background: #F5F6F7;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		margin-top: 20rpx;
		margin-left: 30rpx;
		display: flex;
		align-items: center;
	}
	.tousu-information-three-img{
		width: 44rpx;
		height: 44rpx;
		margin-left: 40rpx;
	}
	.tousu-information-three-input2{
		margin-left: 20rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #666666;
		line-height: 33rpx;
	}
	.tousu-information-three-pl-yi{
		display: flex;
		align-items: center;
		margin-top: 30rpx;
		margin-left: 30rpx;
	}
	.tousu-information-three-pl-yi-img{
		width: 72rpx;
		height: 72rpx;
	}
	.tousu-information-three-pl-yi-text{
		margin-left: 20rpx;
		height: 58rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 58rpx;
	}
	.tousu-information-three-pl-yi-sz{
		margin-left: 284rpx;
		width: 130rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 33rpx;
		text-align: right;
		margin-top: 10rpx;
	}
	.tousu-information-three-pl-yi-img2{
		width: 44rpx;
		height: 44rpx;
		margin-left: 10rpx;
	}
	.tousu-information-three-pl-er{
		margin-left: 120rpx;
		width: 600rpx;
		height: 80rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 38rpx;
	}
	.tousu-information-three-pl-san{
		display: flex;
		align-items: center;
		margin-top: 20rpx;
		margin-left: 120rpx;
	}
	.tousu-information-three-pl-san-text1{
		height: 44rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
		line-height: 33rpx;
	}
	.tousu-information-three-pl-san-text2{
		height: 44rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
	}
	.tousu-information-three-pl-san-img{
		width: 44rpx;
		height: 44rpx;
		margin-left: 330rpx;
	}
	.tousu-information-three-pl-si{
		width: 598rpx;
		height: 208rpx;
		background: #F5F5F5;
		border-radius: 20rpx 20rpx 20rpx 20rpx;
		opacity: 1;
		margin-top: 20rpx;
		margin-left: 120rpx;
	}
	.tousu-information-three-pl-si-text{
		width: 540rpx;
		height: 60rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 38rpx;
		margin: 0 0rpx 0 28rpx;
		padding-top: 20rpx;
	}
	.tousu-information-three-pl-si-text2{
		margin-top: 70rpx;
		margin-left: 28rpx;
		display: flex;
		align-items: center;
	}
	.tousu-information-three-pl-si-text2-t1{
		width: 540rpx;
		height: 44rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
		line-height: 44rpx;
	}
	.tousu-information-three-pl-si-text2-img{
		width: 34rpx;
		height: 34rpx;
	}
	.tousu-information-three-pl-wu{
		height: 66rpx;
		background-color: #FFFFFF;
		display: flex;
		align-items: center;
		justify-content: center;
	}
	.tousu-information-three-pl-wu-text{
		width: 168rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 33rpx;
	}
	.tousu-information-three-pl-wu-img{
		width: 44rpx;
		height: 44rpx;
		margin-left: 10rpx;
	}
</style>