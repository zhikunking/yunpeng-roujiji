<template>
	<view class="tousu">
		<view class="tousu-top">
			<view class="tousu-top-type">投诉类型*</view>
			<view class="tousu-top-right">
				<view class="tousu-top-right-t1">请选择</view>
				<image class="tousu-top-right-t2" src="" mode=""></image>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
	  data() {
	    return {
			
	    };
	  },
	  methods: {
	    
	  },
	};
</script>

<style>
	.tousu{
		width: 100%;
		height: 1804rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.tousu-top{
		/* width: 750rpx; */
		width: 100%;
		height: 104rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		/* padding: 30rpx 40rpx; */
		padding-left: 30rpx;
		display: flex;
		line-height: 104rpx;
	}
	.tousu-top-type{
		width: 146rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 38rpx;
	}
	.tousu-top-right{
		
	}
</style>