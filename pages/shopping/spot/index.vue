<template>
	<view class="spot">
		<uni-nav-bar class="topTabar" title="现货商城" left-icon="left" right-icon="search"></uni-nav-bar>
		<view class="spot-nav">
			<uni-segmented-control :current="current" :values="list1" @clickItem="onClickItem" styleType="text"></uni-segmented-control>
			<ShoppNav v-if="current == 0"/>
			<!-- <ShoppList v-if="current == 0"/> -->
			<ShoppList v-if="current == 1"/>
		</view>
	</view>
</template>

<script>
	import ShoppList from "@/pages/shopping/shopp-list.vue"
	import ShoppNav from "@/pages/shopping/shoppNav.vue"
	export default {
		components:{
			ShoppList,
			ShoppNav
		},
		data() {
			return {
				active:1,
				  list1: ['商品','店铺'],
					current: 0,
				}
		},
		onLoad() {
				
		},
		methods: {
			  qh(index) {
			        this.current = index.index;
			    },
				 onClickItem(e) {
				      if (this.current != e.currentIndex) {
				        this.current = e.currentIndex;
				      }
				    }
		},
	}
</script>
<style>
	.spot{
		width: 100%;
		height: 1624rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		position: relative;
	}
	.spot-nav{
		width: 100%;
		height: 88rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		z-index: 9999999;
		position: absolute;
	}
	.topTabar{
		z-index: 999999;
	}
</style>