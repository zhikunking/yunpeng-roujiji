<template>
	<view class="footmark">
		<view class="footmark_top">
			<view class="footmark_top_day">
				<view class="footmark_top_day_text">
					今天
				</view>
				<image class="footmark_top_day_img" src="../../static/img/di.png" mode=""></image>
			</view>
		</view>
		<view class="footmark_list">
			<view class="footmark_list_root" v-for="(item,index) in list" :key="index">
				<image class="footmark_list_root_img" :src="item.url" mode=""></image>
				<view class="footmark_list_root_text">
					{{item.text}}
				</view>
			</view>
		</view>
	</view>
</template>

<script>
	export default{
		data(){
			return{
				list:[
					{
						url:'../../static/img/root2.png',
						text:'￥100.00'
					},
					{
						url:'../../static/img/root2.png',
						text:'￥100.00'
					},
					{
						url:'../../static/img/root2.png',
						text:'￥100.00'
					},
					{
						url:'../../static/img/root2.png',
						text:'￥100.00'
					},
					{
						url:'../../static/img/root2.png',
						text:'￥100.00'
					},
					{
						url:'../../static/img/root2.png',
						text:'￥100.00'
					},
					{
						url:'../../static/img/root2.png',
						text:'￥100.00'
					},
					{
						url:'../../static/img/root2.png',
						text:'￥100.00'
					},
					{
						url:'../../static/img/root2.png',
						text:'￥100.00'
					},
					{
						url:'../../static/img/root2.png',
						text:'￥100.00'
					},
					{
						url:'../../static/img/root2.png',
						text:'￥100.00'
					},
					{
						url:'../../static/img/root2.png',
						text:'￥100.00'
					},
				]
			}
		}
	}
</script>

<style>
	.footmark{
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
	}
	.footmark_top{
		height: 48rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		padding: 20rpx 0 20rpx 30rpx;
		border-bottom: 2rpx solid #f7f7f7;
		border-top: 2rpx solid #f7f7f7;
	}
	.footmark_top_day{
		width: 128rpx;
		height: 48rpx;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		border: 2rpx solid #C1C1C1;
		
		display: flex;
		align-items: center;
	}
	.footmark_top_day_text{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		margin-left: 22rpx;
	}
	.footmark_top_day_img{
		width: 32rpx;
		height: 32rpx;
	}
	.footmark_list{
		height: 1288rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		padding: 20rpx 30rpx;
		display: flex;
		justify-content: space-evenly;
		flex-wrap: wrap;
	}
	.footmark_list_root{
		height: 238rpx;
		margin-bottom: 30rpx;
	}
	.footmark_list_root_img{
		width: 218rpx;
		height: 218rpx;
	}
	.footmark_list_root_text{
		height: 34rpx;
		font-size: 32rpx;
		font-family: DIN-Bold, DIN;
		font-weight: bold;
		color: #C80000;
		line-height: 38rpx;
		margin-top: 20rpx;
	}
</style>