<template>
	<view class="submit">
		<view class="submit-nav">
			<uni-segmented-control :current="current" :values="list" @clickItem="onClickItem" styleType="button"></uni-segmented-control>
			<view v-show="current === 0">
				<view class="dizhi">
					<view class="dizhi_yi">
						<view class="dizhi_yi_text">
							添加地址
						</view>
						<image class="dizhi_yi_img" src="../../static/img/you.png" mode=""></image>
					</view>
					<view class="dizhi_yi">
						<view class="dizhi_yi_text">
							要货时间
						</view>
						<view class="dizhi_yi_right">
							<view class="dizhi_yi_right_text">
								选择时间
							</view>
							<image class="dizhi_yi_img" src="../../static/img/you.png" mode=""></image>
						</view>
					</view>
				</view>
						<tijiao />
						<view class="shop-bill">
								<view class="dizhi_yi">
									<view class="addzhisj3">开具发票（选填）</view>
									<image class="you" src="../../static/img/you.png" mode=""></image>
								</view>
						</view>
						<view class="shop-remarks">
								<view class="shop-remarks-bz">
									备注
								</view>
								<view class="shop-remarks-input">
									<input class="shop-remarks-input1" type="text" placeholder="请输入">
									<view class="shop-remarks-text2">0/100</view>
								</view>
								
						</view>
						<kefu />
						<tijiaod/>
			</view>
			<view v-show="current === 1">
				<view class="dizhi">
					<view class="dizhi_yi">
						<view class="dizhi_yi_text">
							添加地址1
						</view>
						<image class="dizhi_yi_img" src="../../static/img/you.png" mode=""></image>
					</view>
					<view class="dizhi_yi">
						<view class="dizhi_yi_text">
							要货时间
						</view>
						<view class="dizhi_yi_right">
							<view class="dizhi_yi_right_text">
								选择时间
							</view>
							<image class="dizhi_yi_img" src="../../static/img/you.png" mode=""></image>
						</view>
					</view>
				</view>
						<tijiao />
						<view class="shop-bill">
								<view class="dizhi_yi">
									<view class="addzhisj3">开具发票（选填）</view>
									<view class="addzhisj4">
										<view class="addzhisj4_t1">
											未设置
										</view>
										<image class="you" src="../../static/img/you.png" mode=""></image>
									</view>
								</view>
						</view>
						<view class="shop-remarks">
								<view class="shop-remarks-bz">
									备注
								</view>
								<view class="shop-remarks-input">
									<input class="shop-remarks-input1" type="text" placeholder="请输入">
									<view class="shop-remarks-text2">0/100</view>
								</view>
								
						</view>
						<kefu />
						<tijiaod/>
			</view>
		</view>
	</view>
</template>

<script>
	import tijiao from "@/pages/submit/indextijiao4.vue"
	import kefu from "@/pages/submit/kefu.vue"
	import tijiaod from "@/pages/submit/tijiaodingdan.vue"
	export default {
		components:{
			tijiao,
			kefu,
			tijiaod
		},
	  data() {
	    return {
		   list: ['厂家配送', '自提'],
		    current: 0
	    };
	  },
	  methods:{
		  onClickItem(e) {
			  console.log(e)
		        if (this.current != e.currentIndex) {
		          this.current = e.currentIndex;
		        }
		      }
	  }
	};
</script>

<style>
	.addzhisj4{
		display: flex;
	}
	.addzhisj4_t1{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
		line-height: 33rpx;
		margin-top: 6rpx;
	}
	.shop-remarks-input1{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
		line-height: 33rpx;
	}
	.dizhi{
		margin-bottom: 20rpx;
		height: 176rpx;
		background: #FFFFFF;
		margin-left:30rpx;
		margin-right: 20rpx;
	}
	.dizhi_yi_right_text{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
		line-height: 33rpx;
	}
	.dizhi_yi_right{
		display: flex;
	}
	.dizhi_yi_right_text{
		margin-top: 8rpx;
	}
	.dizhi_yi{
		height: 84rpx;
		display: flex;
		align-items: center;
		justify-content: space-between;
	}
	.dizhi_yi_text{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 38rpx;
	}
	.dizhi_yi_img{
		width: 44rpx;
		height: 44rpx;
	}
	.addzhisj1{
		width: 128rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 38rpx;
	}
	.addzhisj2{
		width: 112rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 33rpx;
	}
	.addzhisj3{
		width: 256rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 38rpx;
		margin-left: 30rpx;
	}
	.you{
		width: 44rpx;
		height: 44rpx;
		margin-right: 20rpx;
	}
	.submit{
		width: 100%;
		height: 1624rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.submit-nav{
		width: 690rpx;
		height: 248rpx;
		background: #FFFFFF;
		border-radius: 20rpx 20rpx 20rpx 20rpx;
		opacity: 1;
		margin-left: 30rpx;
	}
	.submit-nav-song{
		width: 346rpx;
		height: 72rpx;
		background: #3891ED;
		border-radius: 20rpx 0rpx 0rpx 0rpx;
		opacity: 1;
	}
	.shop-bill{
		width: 690rpx;
		height: 82rpx;
		background: #FFFFFF;
		border-radius: 12rpx 12rpx 12rpx 12rpx;
		opacity: 1;
		margin-top: 20rpx;
	}
	.shop-remarks{
		margin-top: 20rpx;
		width: 690rpx;
		height: 244rpx;
		background: #FFFFFF;
		border-radius: 12rpx 12rpx 12rpx 12rpx;
		opacity: 1;
	}
	.shop-remarks-bz{
		height: 104rpx;
		line-height: 104rpx;
		padding-left: 30rpx;
		border-bottom: 2rpx solid #f7f7f7;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
	}
	.shop-remarks-input{
		margin-left: 30rpx;
		margin-top: 20rpx;
	}
	.shop-remarks-text2{
		width: 76rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
		line-height: 32rpx;
		margin-top: 30rpx;
		margin-left: 530rpx;
	}
	.shop-bottom{
		width: 100%;
		height: 112rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		display: flex;
		align-items: center;
	}
	.shop-bottom-text1{
		width: 280rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #C80000;
		line-height: 38rpx;
		margin-left: 30rpx;
	}
	.shop-bottom-text2{
		width: 210rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 32rpx;
	}
	.addzhi{
		width: 64px;
		height: 22px;
		font-size: 16px;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 19px;
	}
</style>