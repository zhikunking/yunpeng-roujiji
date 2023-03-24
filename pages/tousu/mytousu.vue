<template>
	<view class="my-tousu">
		<myTousu />
	</view>
</template>

<script>
	import myTousu from "@/pages/tousu/fztousu.vue"
	export default{
		components:{
			myTousu
		},
		data(){
			return{
				
			}
		}
	}
</script>

<style>
	.my-tousu{
		width: 100%;
		height: 1624rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
</style>