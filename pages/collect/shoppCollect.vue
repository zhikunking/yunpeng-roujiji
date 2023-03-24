<template>
	<view class="collect">
		<view class="collect_tabs">
			<uni-segmented-control :current="current" :values="items" @clickItem="onClickItem" styleType="text"></uni-segmented-control>
		</view>
		<ShoppList />
	</view>
</template>

<script>
	import ShoppList from "@/pages/shopping/shopp-list.vue"
	export default {
		components:{
			ShoppList
		},
	  data() {
	    return {
	        items: ['现货产品', '期货产品'],
	        current: 0
	    };
	  },
	  
	  methods: {
	    onClickItem(e) {
	      if (this.current != e.currentIndex) {
	        this.current = e.currentIndex;
	      }
	    }
	  },
	}
</script>

<style>
	.collect{
		height: 1624rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.collect_tabs{
		height: 88rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
	}
</style>