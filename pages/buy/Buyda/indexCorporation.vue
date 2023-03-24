<template>
	<view class="spot">
		<ShoppNavThree />
		<SearcgCorporation />
	</view>
</template>

<script>
	import SearcgCorporation from "@/pages/search/searcgCorporation.vue"
	import ShoppNavThree from "@/pages/shopping/shoppNavthree.vue"
	export default {
		components:{
			SearcgCorporation,
			ShoppNavThree
		},
		data() {
			return {
				
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
</style>