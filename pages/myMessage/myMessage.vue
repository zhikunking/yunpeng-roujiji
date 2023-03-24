<template>
	<view class="message">
		<view class="message_top" v-for="item in list" :key="item.id">
			<image class="message_top_img" :src="item.url" mode=""></image>
			<view class="message_top_text">
				{{item.name}}
			</view>
		</view>
		<view class="message_title">
			系统公告
		</view>
		<view class="message_list" v-for="item in list1" :key="item.id">
			<view class="message_list-title">
				<view class="message_list-title1">
					{{item.name1}}
				</view>
				<view class="message_list-red"></view>
			</view>
			<view class="message_list-title2">
				{{item.name2}}
			</view>
			<view class="message_list-title3">
				<view class="message_list-title3-t1">
					{{item.name3}}
				</view>
				<view class="message_list-title3-t2">
					<view class="message_list-title3-t2-title">
						{{item.name4}}
					</view>
					<image class="message_list-title3-t2-img" :src="item.url"></image>
				</view>
			</view>
		</view>
		<view class="message_bottom">
			<view class="message_bottom-text">
				查看详情
			</view>
			<image class="message_bottom-img" src="../../static/img/rights.png"></image>
		</view>
	</view>
</template>

<script>
	export default{
		data(){
			return{
				list:[
					{
						url:'../../static/img/xiaoxi.png',
						id:0,
						name:'收到的回复'
					},
					{
						url:'../../static/img/zan3.png',
						id:1,
						name:'收到的赞'
					},
					{
						url:'../../static/img/status.png',
						id:2,
						name:'我的投诉'
					},
				],
				list1:[
					{
						url:'../../static/img/rights.png',
						id:0,
						name1:'【系统通知】平台公告',
						name2:'这里是内容这里是内容这里是内容这里是内容这里是内容这里是内容这里是内容',
						name3:'2019-03-21',
						name4:'查看详情'
					},
					{
						url:'../../static/img/rights.png',
						id:1,
						name1:'【系统通知】平台公告',
						name2:'这里是内容这里是内容这里是内容这里是内容这里是内容这里是内容这里是内容',
						name3:'2019-03-21',
						name4:'查看详情'
					}
				]
			}
		}
	}
</script>

<style>
	.message{
		height: 1624rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.message_top{
		height: 104rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		display: flex;
		align-items: center;
		border-bottom: 2rpx solid #F8F8F8;
	}
	.message_top:last-child{
		border: none;
	}
	.message_top_img{
		width: 48rpx;
		height: 48rpx;
		margin-left: 30rpx;
	}
	.message_top_text{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 38rpx;
		margin-left: 30rpx;
	}
	.message_top_border{
		height: 104rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		display: flex;
		align-items: center;
		border-top: 2rpx solid #F8F8F8;
		border-bottom: 2rpx solid #F8F8F8;
	}
	.message_title{
		margin: 30rpx 0 30rpx 30rpx;
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Bold, PingFang SC;
		font-weight: bold;
		color: #000000;
		line-height: 38rpx;
	}
	.message_list{
		margin: 0 30rpx 20rpx 30rpx;
		height: 294rpx;
		background: #FFFFFF;
		border-radius: 20rpx 20rpx 20rpx 20rpx;
		opacity: 1;
	}
	.message_list-title{
		padding-top: 30rpx;
		display: flex;
		align-items: center;
	}
	.message_list-title1{
		margin: 0rpx 0 30rpx 20rpx;
	}
	.message_list-red{
		width: 20rpx;
		height: 20rpx;
		background: #DB0D0D;
		opacity: 1;
		margin-bottom: 24rpx;
		border-radius: 50%;
		margin-left: 20rpx;
	}	
	.message_list-title2{
		margin: 0 20rpx 20rpx 20rpx;
		width: 650rpx;
		height: 100rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #666666;
		line-height: 50rpx;
	}
	.message_list-title3{
		display: flex;
		align-items: center;
		justify-content: space-between;
		margin: 20rpx 20rpx 30rpx 20rpx;
	}
	.message_list-title3-t1{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #666666;
		line-height: 33rpx;
	}
	.message_list-title3-t2{
		display: flex;
		height: 40rpx;
		align-items: center;
	}
	.message_list-title3-t2-title{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #666666;
		line-height: 33rpx;
	}
	.message_list-title3-t2-img{
		width: 40rpx;
		height: 40rpx;
		margin-bottom: 10rpx;
	}
	.message_bottom{
		width: 100%;
		height: 40rpx;
		display: flex;
		align-items: center;
		justify-content: center;
		margin-top: 40rpx;
	}
	.message_bottom-text{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #666666;
		line-height: 33rpx;
		text-align: center;
	}
	.message_bottom-img{
		width: 40rpx;
		height: 40rpx;
		margin-bottom: 10rpx;
		/* display: block; */
		/* margin: 0 auto; */
	}
</style>