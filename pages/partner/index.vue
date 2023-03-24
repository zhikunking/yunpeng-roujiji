<template>
	<view class="partner">
		<view class="partner_top">
			<view class="partner_top_text">
				<p>申请须知</p>
				<p>云蓬以长远的眼光、诚信负责的操守、共同成长的理念，发展公司的事业，坚持“用户第一”理念。 公司以新颖的开发作为肩负的责任，通过精美的各类特色服务客户，满足每一个客户的荣耀与梦想，我们珍惜每次一次为客户服务的机会，以感激的心态对待客户的关注、选择和信任。我们注重每一个服务过程和细节的完美，用心服务，用情感人，想客户所想，急客户所需，力求超越客户的期望价值。云蓬成功帮助多家知名互联网公司获得多轮融资。专注于手机APP定制开发、高端网站定制、企业网站建设、手机移动网站建设、应用系统开发、物联网开发等，为企业提供全球化互联网解决方案。公司自创立以来，已成功为数百余家企事业单位、政府机关提供过高端互联网。物联网服务。</p>
			</view>
		</view>
		<view class="partner_bottom">
			<view class="authentication_name">
				<view class="authentication_name_text">
					联系人：
				</view>
				<input style="margin-left:32rpx" class="authentication_name_input" type="text" placeholder="请输入">
			</view>
			<view class="authentication_name">
				<view class="authentication_name_text">
					联系方式：
				</view>
				<input class="authentication_name_input" type="text" placeholder="请输入">
			</view>
		</view>
		<view class="partner_btn">
			确认提交
		</view>
	</view>
</template>

<script>
</script>

<style>
	.partner{
		height: 1424rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		position: relative;
	}
	.partner_top{
		height: 676rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		padding: 30rpx 40rpx 38rpx 40rpx;
	}
	.partner_top_text{
		width: 670rpx;
		height: 666rpx;
		font-size: 30rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 44rpx;
	}
	.partner_bottom{
		margin-top: 20rpx;
	}
	.authentication_name{
		height: 44rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		padding: 30rpx;
		display: flex;
		align-items: center;
		border-bottom: 2rpx solid #f6f6f6;
	}
	.authentication_name_text{
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #333333;
		line-height: 38rpx;
	}
	.authentication_name_input{
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
		line-height: 33rpx;
	}
	.partner_btn{
		position: absolute;
		bottom: 0;
		margin-bottom: 40rpx;
		margin-left: 30rpx;
		width: 690rpx;
		height: 88rpx;
		background: #3891ED;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #FFFFFF;
		line-height: 88rpx;
		text-align: center;
	}
	
</style>