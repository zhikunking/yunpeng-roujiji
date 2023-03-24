<template>
	<view class="corporation">
		<view class="spot-list" v-for="(item,index) in corporationList" :key="index">
			<view class="spot-list-text1">
				{{item.name1}}
			</view>
			<view class="spot-list-text2">
				{{item.name2}}
			</view>
			<view class="spot-list-text2">
				{{item.name3}}
			</view>
			<view class="spot-list-text2">
				{{item.name4}}
			</view>
			<u-divider />
			<view class="spot-list-corporation">
				<view class="spot-list-corporation-t1">
					{{item.name5}}
				</view>
				<image class="spot-list-corporation-img1" :src="item.url1" mode=""></image>
				<image class="spot-list-corporation-img2" :src="item.url2" mode=""></image>
				<view class="spot-list-corporation-t2">
					{{item.name6}}
				</view>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
	  data() {
	    return {
	      corporationList:[
			  {
				  name1:'山东肉集集信息科技有限责任公司',
				  name2:'注册时间：2022年12月3日',
				  name3:'主营产品：猪产品、牛产品、鸡产品',
				  name4:'店铺起售量：100千克',
				  name5:'黑龙江哈尔滨食品有限公司',
				  name6:'5km',
				  url1:'../../static/img/geren.png',
				  url2:'../../static/img/fuzhi.png'
			  },
			  {
			  	name1:'山东肉集集信息科技有限责任公司',
			  	name2:'注册时间：2022年12月3日',
			  	name3:'主营产品：猪产品、牛产品、鸡产品',
			  	name4:'店铺起售量：100千克',
			  	name5:'黑龙江哈尔滨食品有限公司',
			  	name6:'5km',
				url1:'../../static/img/qiye.png',
				url2:'../../static/img/fuzhi.png'
			  },
			  {
			  	name1:'山东肉集集信息科技有限责任公司',
			  	name2:'注册时间：2022年12月3日',
			  	name3:'主营产品：猪产品、牛产品、鸡产品',
			  	name4:'店铺起售量：100千克',
			  	name5:'黑龙江哈尔滨食品有限公司',
			  	name6:'5km',
			  	url1:'../../static/img/geti.png',
			  	url2:'../../static/img/fuzhi.png'
			  },
		  ]
	    };
	  },
	  methods: {
	    
	  },
	};
</script>

<style>
	.spot-list{
		width: 686rpx;
		/* height: 372rpx; */
		background: #FFFFFF;
		border-radius: 20rpx 20rpx 20rpx 20rpx;
		opacity: 1;
		margin-top: 20rpx;
		margin-left: 30rpx;
	}
	.spot-list-text1{
		width: 480rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 38rpx;
		padding-top: 30rpx;
		margin-left: 30rpx;
	}
	.spot-list-text2{
		width: 448rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #666666;
		line-height: 33rpx;
		margin-left: 30rpx;
		margin-top: 8rpx;
	}
	.spot-list-text3{
		display: flex;
	}
	.spot-list-text3-one2{
		width: 2rpx;
		opacity: 1;
		height: 70rpx;
		background-color: #CCCCCC;
		margin-left: 98rpx;
	}
	.spot-list-text3-one1-t1{
		width: 146rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
		margin-left: 100rpx;
	}
	.spot-list-text3-one1-t2{
		width: 146rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
		margin-left: 100rpx;
		text-align: center;
	}
	.spot-list-corporation{
		display: flex;
		align-items: center;
		margin-left: 30rpx;
		padding-bottom: 30rpx;
	}
	.spot-list-corporation-t1{
		width: 336rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #333333;
		line-height: 33rpx;
	}
	.spot-list-corporation-img1{
		width: 92rpx;
		height: 50rpx;
		margin-left: 20rpx;
	}
	.spot-list-corporation-img2{
		width: 40rpx;
		height: 40rpx;
		margin-left: 10rpx;
	}
	.spot-list-corporation-t2{
		width: 56rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 40rpx;
		margin-left: 78rpx;
	}
</style>