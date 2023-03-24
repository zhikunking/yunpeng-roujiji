<template>
	<view class="manage-address">
		<view class="manage-address-top">
			<view class="manage-address-top-text1">
				张晓伟 186****2128
			</view>
			<view class="manage-address-top-text2">
				ARKANSAS Aberdenn,详细地址
			</view>
			<view class="manage-address-top-text2">
				19929928882@172.com     658279
			</view>
			<view class="manage-address-top-text3"></view>
			<view class="manage-address-top-bottom">
				<view class="manage-address-top-bottom-box1">
					<image @click="iSshowStatus" v-if="iSshow == false" class="manage-address-top-bottom-box1-img" src="../../static/img/yuan1.png" mode=""></image>
					<image @click="iSshowStatus" v-if="iSshow == true" class="manage-address-top-bottom-box1-img" src="../../static/img/yuan2.png" mode=""></image>
					<view class="manage-address-top-bottom-box1-text">
						默认
					</view>
				</view>
				<view class="manage-address-top-bottom-box2">
					<image class="manage-address-top-bottom-box2-img" src="../../static/img/edit2.png" mode=""></image>
					<view class="manage-address-top-bottom-box2-text">
						编辑
					</view>
				</view>
				<view class="manage-address-top-bottom-box3">
					<image class="manage-address-top-bottom-box3-img" src="../../static/img/del3.png" mode=""></image>
					<view class="manage-address-top-bottom-box3-text">
						编辑
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
				iSshow:true
			}
		},
		methods:{
			iSshowStatus(){
				this.iSshow =! this.iSshow
			},
		}
	}
</script>

<style>
	.manage-address{
		height: 1624rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.manage-address-top{
		height: 300rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		border-top: 2rpx solid #F5F6F7;
	}
	.manage-address-top-text1{
		padding-top: 30rpx;
		margin-left: 30rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 33rpx;
	}
	.manage-address-top-text2{
		margin-top: 12rpx;
		margin-left: 30rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #666666;
		line-height: 33rpx;
	}
	.manage-address-top-text3{
		margin-left: 28rpx;
		margin-right: 32rpx;
		margin-top: 30rpx;
		margin-bottom: 14rpx;
		width: 690rpx;
		height: 0rpx;
		opacity: 1;
		border: 2rpx solid #F5F6F7;
	}
	.manage-address-top-bottom{
		display: flex;
		align-items: center;
		height: 66rpx;
	}
	.manage-address-top-bottom-box1{
		display: flex;
		align-items: center;
	}
	.manage-address-top-bottom-box1-img{
		width: 48rpx;
		height: 48rpx;
		margin-left: 24rpx;
	}
	.manage-address-top-bottom-box1-text{
		/* width: 56rpx; */
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #999999;
		line-height: 33rpx;
		margin-left: 8rpx;
		margin-top: 8rpx;
	}
	.manage-address-top-bottom-box2{
		display: flex;
		align-items: center;
		
	}
	.manage-address-top-bottom-box2-img{
		width: 44rpx;
		height: 44rpx;
		margin-left: 308rpx;
	}
	.manage-address-top-bottom-box2-text{
		width: 56rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #999999;
		line-height: 33rpx;
		margin-top: 8rpx;
	}
	.manage-address-top-bottom-box3{
		display: flex;
		align-items: center;
	}
	.manage-address-top-bottom-box3-img{
		width: 48rpx;
		height: 48rpx;
		margin-left: 60rpx;
	}
	.manage-address-top-bottom-box3-text{
		width: 56rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #999999;
		line-height: 33rpx;
		margin-top: 8rpx;
	}
</style>