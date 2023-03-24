<template>
	<view class="spot">
		<u-tabs :list="list1">
				<ShoppNavTwo />
				<ShoppList />
			<!-- <u-tab title="店铺"> -->
				<!-- <van-dropdown-menu>
					<van-dropdown-item title="区域">
						<view class="spot-seat1">
							当前国家：郑州 | 重新定位
						</view>
						<view class="spot-seat2">
							<view class="spot-seat2-btn" v-for="(item,index) in text" :key="index">
								{{item}}
							</view>
						 </view>
						 <van-area title="标题" :area-list="areaList" />
					</van-dropdown-item>
				</van-dropdown-menu>
				<view class="spot-list">
					<view class="spot-list-text1">
						山东肉集集信息科技有限责任公司
					</view>
					<view class="spot-list-text2">
						注册时间：2022年12月3日
					</view>
					<view class="spot-list-text2">
						主营产品：猪产品、牛产品、鸡产品
					</view>
					<view class="spot-list-text2">
						店铺起售量：100千克
					</view>
					<van-divider />
					<view class="spot-list-text3">
						<view class="spot-list-text3-one1">
							<view class="spot-list-text3-one1-t1">
								近30天报价
							</view>
							<view class="spot-list-text3-one1-t2">
								90
							</view>
						</view>
						<view class="spot-list-text3-one2">
							
						</view>
						<view class="spot-list-text3-one1">
							<view class="spot-list-text3-one1-t1">
								累计成交
							</view>
							<view class="spot-list-text3-one1-t2">
								0
							</view>
						</view>
					</view>
				</view> -->
			<!-- </u-tab> -->
		</u-tabs>
	</view>
</template>

<script>
	import ShoppList from "@/pages/shopping/shopp-list.vue"
	import ShoppNavTwo from "@/pages/shopping/shoppNavTwo.vue"
	export default {
		components:{
			ShoppList,
			ShoppNavTwo
		},
		data() {
			return {
				active:1,
				list1: [
					{
				        name: '商品',
				    }, 
					{
				        name: '店铺',
				    }
				],
				text:['全广东','100km','200km','500km','800km'],
				list: ['猪产品','牛产品','鸡产品','鸭产品','水产品','羊产品','其他'],
				list1: ['不限','鲜品','冻品'],
				list2: ['价格优先','距离优先','销量优先'],
				list3: ['不限','公','母'],
				list4: ['不限','鲜品','冻品'],
				list5: ['不限','中国','巴西','西班牙','德国','美国','荷兰','丹麦','印尼','日本','韩国','法国'],
			}
		},
		onLoad() {
				
		},
		methods: {
			
		},
	}
</script>
<style>
	.spot{
		width: 100%;
		height: 1624rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.spot-nav{
		width: 100%;
		height: 88rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
	
	}
	.content {
		display: flex;
		justify-content: center;
		align-items: center;
		height: 300rpx;
		text-align: center;
	}
	.spot-seat1{
		width: 352rpx;
		height: 50rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 50rpx;
		margin-left: 30rpx;
	}
	.spot-seat2{
		width: 100%;
		height: 60rpx;
		line-height: 60rpx;
		display: flex;
		margin-top: 24rpx;
		margin-left: 20rpx;
		margin-bottom: 30rpx;
		margin-right: 28rpx;
	}
	.spot-seat2-btn{
		width: 132rpx;
		height: 60rpx;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		border: 2rpx solid #999999;
		text-align: center;
		margin-left: 10rpx;
		font-family: PingFang SC-Regular;
		font-weight: Regular;
		font-size: 28rpx;
		color: #666666;
	}
	.spot-list{
		width: 686rpx;
		height: 372rpx;
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
</style>