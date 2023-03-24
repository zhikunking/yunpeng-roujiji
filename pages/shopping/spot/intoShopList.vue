<template>
	<view class="info-shop">
		<view class="info-shop-banner">
			
		</view>
		<view class="info-shop-name">
			<view class="info-shop-name-text1">
				商品名称
			</view>
			<view class="info-shop-name-text2">
				29~39元/千克
			</view>
			<view class="info-shop-name-text3">
				<view class="info-shop-name-text3-t1">
					单商品加购量：5千克
				</view>
				<view class="info-shop-name-text3-t2">
					店铺总起售量：500千克
				</view>
			</view>
			<view class="info-shop-name-text4">
				<view class="info-shop-name-text4-t1">
					更新时间:2022-10-27
				</view>
				<view class="info-shop-name-text4-t2">
					猪产品
				</view>
			</view>
		</view>
		<view class="info-shop-address">
			<image class="info-shop-address-t1" src="../../../static/img/weizhi.png"></image>
			<view class="info-shop-address-t2">
				广东省深圳市南山
			</view>
			<view class="info-shop-address-t3">
				距您1011km
			</view>
		</view>
		<view class="info-shop-classify">
			<view class="info-shop-classify-xinx">
				<view class="info-shop-classify-xinx-t1">
					商品分类
				</view>
				<view class="info-shop-classify-xinx-t2">
					查看所有
				</view>
			</view>
			<view class="info-shop-classify-list" v-for="(item,index) in list" :key="index">
				<image class="info-shop-classify-list1" :src="item.url" mode=""></image>
				<view class="info-shop-classify-list2">{{item.name1}}</view>
				<view class="info-shop-classify-list3">{{item.name2}}</view>
			</view>
		</view>
		<view class="info-shop-information">
			<u-cell-group>
					<u-cell>
						<template #title>
							<view class="info-shop-information-text">
								<view class="info-shop-information-text1">店铺信息</view>
								<view class="info-shop-information-text2" @click="jindian">进店</view>
								<image class="info-shop-information-text3" src="../../../static/img/right.png" mode=""></image>
							</view>
						</template>
					</u-cell>
					<u-cell>
						<template #title>
							<view class="info-shop-information-img">
								<image class="info-shop-information-img1" src="../../../static/img/tupian.png"></image>
								<view class="info-shop-information-img2">黑龙江哈尔滨食品有限公司</view>
								<image class="info-shop-information-img3" src="../../../static/img/qiye.png" mode=""></image>
							</view>
							<view class="info-shop-information-btn">联系商家</view>
						</template>
					</u-cell>
			</u-cell-group>
		</view>
		<view class="info-shop-recommend">
			<u-cell-group>
					<u-cell>
						<template #title>
							<view class="info-shop-information-text">
								<view class="info-shop-information-text1">店铺推荐</view>
								<view class="info-shop-recommend-text2">查看全部</view>
								<image class="info-shop-information-text3" src="../../../static/img/right.png" mode=""></image>
							</view>
						</template>
					</u-cell>
					<u-cell>
						<template #title>
							<view class="info-shop-recommend-list">
								<view class="info-shop-recommend-list1" v-for="(item,index) in shoppList" :key="index">
									<image class="info-shop-recommend-list-img" :src="item.url" mode=""></image>
									<view class="info-shop-recommend-list-text1">{{item.text1}}</view>
									<view class="info-shop-recommend-list-text2">{{item.text2}}</view>
								</view>
							</view>
						</template>
					</u-cell>
				</u-cell-group>
		</view>
		<view class="info-shop-info">
			<view class="info-shop-info-top">商品详情</view>
			<image class="info-shop-info-img" src="../../../static/img/jing.png" mode=""></image>
			<view class="info-shop-info-text">
				手机详情标题内容（4G/5G）全屏智能手机，高清看电影打游戏手机详情标题内容（4G/5G）全屏智能手机，高清看电影打游戏手机详情标题内容（4G/5G）全屏智能手机，高清看电影打游戏手机详情标题内容（4G/5G）全屏智能手机，高清看电影打游戏手机详情标题内容（4G/5G）全屏智能手机，高清看电影打游戏手机详情标题内容（4G/5G）全屏智能手机，高清看电影打游戏
			</view>
		</view>
		<view class="bottom">
			<view class="bottom_btn"></view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				list:[
					{
						url:'../../../static/img/root.png',
						name1:'猪肋排',
						name2:'￥33.5元/千克'
					},
					{
						url:'../../../static/img/root.png',
						name1:'猪肋排',
						name2:'￥33.5元/千克'
					}
				],
				shoppList:[
					{
						url:'../../../static/img/root2.png',
						text1:'商品名称商品名称 商品名称',
						text2:'￥100.00'
					},
					{
						url:'../../../static/img/root2.png',
						text1:'商品名称商品名称 商品名称',
						text2:'￥100.00'
					},
					{
						url:'../../../static/img/root2.png',
						text1:'商品名称商品名称 商品名称',
						text2:'￥100.00'
					},
					{
						url:'../../../static/img/root2.png',
						text1:'商品名称商品名称 商品名称',
						text2:'￥100.00'
					},
					{
						url:'../../../static/img/root2.png',
						text1:'商品名称商品名称 商品名称',
						text2:'￥100.00'
					},
					{
						url:'../../../static/img/root2.png',
						text1:'商品名称商品名称 商品名称',
						text2:'￥100.00'
					}
				]
			}
		},
		onLoad() {
	
		},
		methods: {
			jindian(){
				uni.navigateTo({
					url:'/pages/shopping/shopp/shoppSheet'
				})
			}
		}
	}
</script>

<style>
	.bottom{
		width: 100%	;
		height: 112rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		position: absolute;
		bottom: 0;
		display: flex;
		
	}
	
	
	.info-shop{
		width: 100%;
		height: 3254rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		position: relative;
	}
	.info-shop-banner{
		width: 100%;
		height: 332rpx;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		/* background-image: url(""); */
		background-size: 100% 100%;
	}
	.info-shop-name{
		width: 100%;
		height: 276rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
	}
	.info-shop-name-text1{
		width: 666rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 38rpx;
		padding: 30rpx;
	}
	.info-shop-name-text2{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #C80000;
		margin-left: 30rpx;
	}
	.info-shop-name-text3{
		display: flex;
		margin-left: 30rpx;
		margin-top: 12rpx;
	}
	.info-shop-name-text3-t1{
		width: 270rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
	}
	.info-shop-name-text3-t2{
		width: 304rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
		margin-left: 100rpx;
	}
	.info-shop-name-text4{
		display: flex;
		margin-top: 12rpx;
		margin-left: 30rpx;
	}
	.info-shop-name-text4-t1{
		width: 282rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
	}
	.info-shop-name-text4-t2{
		width: 84rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
		margin-left: 88rpx;
	}
	.info-shop-address{
		width: 100%;
		height: 100rpx;
		background: #FFFFFF;
		opacity: 1;
		margin-top: 20rpx;
		display: flex;
		align-items: center;
		padding-left: 30rpx;
	}
	.info-shop-address-t1{
		width: 48rpx;
		height: 48rpx;
	}
	.info-shop-address-t2{
		width: 224rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
		margin-left: 15rpx;
	}
	.info-shop-address-t3{
		margin-left: 240rpx;
		width: 166rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
	}
	.info-shop-classify{
		width: 100%;
		height: 314rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		margin-top: 20rpx;
	}
	.info-shop-classify-xinx{
		padding-top: 30rpx;
		margin-left: 30rpx;
		display: flex;
	}
	.info-shop-classify-xinx-t1{
		width: 580rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 38rpx;
	}
	.info-shop-classify-xinx-t2{
		width: 112rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #3891ED;
		line-height: 33rpx;
	}
	.info-shop-classify-list{
		display: flex;
		margin-top: 30rpx;
		margin-left: 30rpx;
	}
	.info-shop-classify-list1{
		width: 80rpx;
		height: 80rpx;
	}
	.info-shop-classify-list2{
		margin-left: 20rpx;
		margin-top: 20rpx;
		width: 84rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
	}
	.info-shop-classify-list3{
		margin-left: 332rpx;
		width: 184rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
		margin-top: 20rpx;
	}
	.info-shop-information{
		margin-top: 20rpx;
		width: 100%;
		height: 314rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
	}
	.info-shop-information-text{
		display: flex;
	}
	.info-shop-information-text1{
		width: 128rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 38rpx;
	}
	.info-shop-information-text2{
		width: 56rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #3891ED;
		line-height: 33rpx;
		margin-left: 230px;
		margin-top: 10rpx;
	}
	.info-shop-information-text3{
		width: 36rpx;
		height: 36rpx;
		margin-top: 9rpx;
	}
	.info-shop-information-img{
		display: flex;
	}
	.info-shop-information-img1{
		width: 112rpx;
		height: 112rpx;
		margin-left: 20rpx;
	}
	.info-shop-information-img2{
		margin-left: 20rpx;
		margin-top: 30rpx;
		width: 384rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 38rpx;
	}
	.info-shop-information-img3{
		width: 92rpx;
		height: 50rpx;
		margin-top: 26rpx;
		margin-left: 20rpx;
	}
	.info-shop-information-btn{
		width: 160rpx;
		height: 64rpx;
		line-height: 64rpx;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		border: 2rpx solid #999999;
		font-family: PingFang SC-Regular;
		font-weight: Regular;
		color: #666666;
		font-size: 28rpx;
		text-align: center;	
		margin-left: 520rpx;
	}
	.info-shop-recommend{
		width: 100%;
		height: 846rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		margin-top: 20rpx;
	}
	.info-shop-recommend-text2{
		width: 116rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #3891ED;
		line-height: 33rpx;
		margin-left: 200px;
		margin-top: 10rpx;
	}
	.info-shop-recommend-list{
		display: flex;
		flex-wrap: wrap;
		width: 100%;
	}
	.info-shop-recommend-list1{
		width: 216rpx;
		height: 336rpx;
		margin-bottom: 20rpx;
		margin-right: 14rpx;
	}
	.info-shop-recommend-list-img{
		width: 216rpx;
		height: 216rpx;
	}
	.info-shop-recommend-list-text1{
		width: 208rpx;
		height: 72rpx;
		font-size: 26rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 30rpx;
		margin-top: 12rpx;
	}
	.info-shop-recommend-list-text2{
		width: 112rpx;
		height: 36rpx;
		font-size: 26rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #C80000;
		line-height: 30rpx;
	}
	.info-shop-info{
		margin-top: 20rpx;
		width: 100%;
		height: 844rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
	}
	.info-shop-info-top{
		padding-top: 30rpx;
		margin-left: 42rpx;
	}
	.info-shop-info-img{
		width: 690rpx;
		height: 360rpx;
		margin: 30rpx;
	}
	.info-shop-info-text{
		margin-left: 30rpx;
		width: 690rpx;
		height: 320rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #000000;
		line-height: 40rpx;
	}
	.info-shop-bottom{
		position: absolute;
		bottom: 0;
		width: 100%;
		height: 112rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
	}
</style>