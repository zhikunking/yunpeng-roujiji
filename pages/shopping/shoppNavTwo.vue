<template>
	<view>
		<!-- <u-dropdown-menu>
			<u-dropdown-item title="生产国家">
				<view class="spot-seat1">
					当前国家：郑州 | 重新定位
				</view>
				<view class="spot-seat2">
					<view class="spot-seat2-btn" v-for="(item,index) in text" :key="index">
						{{item}}
					</view>
				 </view>
				 <u-area title="标题" :area-list="areaList" />
			</u-dropdown-item>
			<u-dropdown-item title="品类">
				<view class="spot-category">
					<view class="spot-category-text">
						品类
					</view>
					<image class="spot-category-img" src="../../static/img/x.png" mode=""></image>
				</view>
				<u-cell v-for="item in list" :key="item" :title="item" />
			</u-dropdown-item>
			<u-dropdown-item title="鲜冻类型">
				<view class="spot-category">
					<view class="spot-category-text2">
						鲜冻类型
					</view>
					<image class="spot-category-img" src="../../static/img/x.png" mode=""></image>
				</view>
				<u-cell v-for="item in list1" :key="item" :title="item" />
			</u-dropdown-item>
			<u-dropdown-item title="排序方式">
				<view class="spot-category">
					<view class="spot-category-text2">
						排序方式
					</view>
					<image class="spot-category-img" src="../../static/img/x.png" mode=""></image>
				</view>
				<u-cell v-for="item in list2" :key="item" :title="item" />
			</u-dropdown-item>
			<u-dropdown-item title="筛选">
				<view class="spot-category">
					<view class="spot-category-text2">
						筛选
					</view>
					<image class="spot-category-img" src="../../static/img/x.png" mode=""></image>
				</view>
				<view class="spot-category2">
					<view class="spot-category2-text">
						公母类型
					</view>
				</view>
				<view class="spot-category3">
					<view class="spot-category2-text2" v-for="item in list3" :key="item">
						{{item}}
					</view>
				</view>
				<view class="spot-category2">
					<view class="spot-category2-text">
						鲜冻类型
					</view>
				</view>
				<view class="spot-category3">
					<view class="spot-category2-text2" v-for="item in list4" :key="item">
						{{item}}
					</view>
				</view>
				<view class="spot-category2">
					<view class="spot-category2-text">
						店铺起售
					</view>
				</view>
				<view class="spot-category3">
					<view class="spot-category2-text3" >
						<input class="spot-category2-inp" type="text"  placeholder="请输入起售量">
					</view>
					<view class="spot-category2-text4">千克</view>
				</view>
				<view class="spot-category4">
					<view>
						生产国家（可多选）
					</view>
					<view class="spot-category4-text5">
						更多
					</view>
				</view>
				<view class="spot-category5">
					<view class="spot-category5-text2" v-for="item in list5" :key="item">
						{{item}}
					</view>
				</view>
				<view class="spot-category6">
					<button class="spot-category6-btn1">重置</button>
					<button class="spot-category6-btn2">确认</button>
				</view>
			</u-dropdown-item>
		</u-dropdown-menu> -->
	</view>
</template>

<script>
	export default {
		components:{
			
		},
		data() {
			return {
				// text:['全广东','100km','200km','500km','800km'],
				// list: ['猪产品','牛产品','鸡产品','鸭产品','水产品','羊产品','其他'],
				// list1: ['不限','鲜品','冻品'],
				// list2: ['价格优先','距离优先','销量优先'],
				// list3: ['不限','公','母'],
				// list4: ['不限','鲜品','冻品'],
				// list5: ['不限','中国','巴西','西班牙','德国','美国','荷兰','丹麦','印尼','日本','韩国','法国'],
			}
		},
		onLoad() {
				
		},
		methods: {
			
		},
	}
</script>

<style>
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
	.spot-category{
		display: flex;
		margin-left: 46rpx;
		margin-bottom: 20rpx;
		margin-right: 38rpx;
		justify-content: space-between;
		align-items: center;
	}
	.spot-category-text{
		width: 64rpx;
		height: 58rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 58rpx;
	}
	.spot-category-img{
		width: 32rpx;
		height: 32rpx;
	}
	.spot-category-text2{
		width: 128rpx;
		height: 58rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 58rpx;
	}
	.spot-category2{
		margin-left: 46rpx;
		margin-bottom: 30rpx;
	}
	.spot-category-text2{
		width: 128rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 38rpx;
	}
	.spot-category3{
		width: 100%;
		margin-left: 20rpx;
		margin-bottom: 42rpx;
		display: flex;
	}
	.spot-category2-text2{
		width: 214rpx;
		height: 72rpx;
		line-height: 72rpx;
		text-align: center;
		border-radius: 12rpx 12rpx 12rpx 12rpx;
		opacity: 1;
		border: 2rpx solid #999999;
		margin-left: 20rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #666666;
	}
	.spot-category2-text3{
		width: 326rpx;
		height: 72rpx;
		border-radius: 12rpx 12rpx 12rpx 12rpx;
		opacity: 1;
		border: 2rpx solid #999999;
		margin-left: 20rpx;
		display: flex;
	}
	.spot-category2-inp{
		margin-top: 10rpx;
		margin-left: 72rpx;
	}
	.spot-category2-text4{
		margin-left: 20rpx;
		width: 78rpx;
		height: 72rpx;
		line-height: 72rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #666666;
	}
	.spot-category4{
		margin-left: 46rpx;
		margin-bottom: 30rpx;
		display: flex;
	}
	.spot-category4-text5{
		margin-left: 312rpx;
		width: 64rpx;
		height: 58rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #3891ED;
	}
	.spot-category5{
		margin-left: 40rpx;
		margin-bottom: 22rpx;
		display: flex;
		flex-wrap: wrap;
	}
	.spot-category5-text2{
		width: 160rpx;
		height: 72rpx;
		line-height: 72rpx;
		text-align: center;
		border-radius: 12rpx 12rpx 12rpx 12rpx;
		opacity: 1;
		border: 2rpx solid #999999;
		margin-left: 10rpx;
		margin-bottom: 20rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #666666;
	}
	.spot-category6{
		width: 100%;
		margin-bottom: 34rpx;
		margin-top: 8rpx;
		display: flex;
	}
	.spot-category6-btn1{
		width: 330rpx;
		height: 88rpx;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		border: 2rpx solid #333333;
	}
	.spot-category6-btn2{
		width: 330rpx;
		height: 88rpx;
		background: #3891ED;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		color: #FFFFFF;
	}
</style>