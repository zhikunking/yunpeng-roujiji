<template>
	<view class="blacklist">
		<image class="blacklist-banner" src="../../static/img/group.png" mode=""></image>
		<view class="blacklist-nav">
			<view class="blacklist-nav-yi">
				 <u-tabs :list="list1" @click="click"></u-tabs>
			</view>
			<image class="blacklist-nav-er" src="../../static/img/Search.png" mode=""></image>
		</view>
		<view class="blacklist-list">
			<myTousu />
		</view>
	</view>
</template>

<script>
	import myTousu from "@/pages/tousu/fztousu.vue"
	export default {
		components:{
			myTousu
		},
			data() {
				return {
	                list1: [{
	                    name: '全部',
	                }, {
	                    name: '放鸽子',
	                }, {
	                    name: '货不对板'
	                }, {
	                    name: '收货不收货'
	                }, {
	                    name: '合同'
	                }]
				}
			},
			methods: {
	            click(item) {
	                console.log('item', item);
	            }
			}
		}
</script>

<style>
	.blacklist{
		width: 100%;
		height: 1624rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.blacklist-banner{
		width: 690rpx;
		height: 240rpx;
		margin-top: 20rpx;
		margin-left: 30rpx;
		margin-right: 30rpx;
	}
	.blacklist-nav{
		display: flex;
		height: 88rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		align-items: center;
	}
	.blacklist-nav-yi{
		margin-right: 30rpx;
	}
	.blacklist-nav-er{
		width: 44rpx;
		height: 44rpx;
		margin-right: 30rpx;
	}
	.blacklist-list{
		margin-top: 20rpx;
	}
</style>