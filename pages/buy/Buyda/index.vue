<template>
	<view class="spot">
		<ShoppNavThree />
		<ShoppList />
	</view>
</template>

<script>
	import ShoppList from "@/pages/shopping/shopp-list.vue"
	import ShoppNavThree from "@/pages/shopping/shoppNavthree.vue"
	export default {
		components:{
			ShoppList,
			ShoppNavThree
		},
		data() {
			return {
				shopList:[
					{
						url1:"../../../static/img/roo2.png",
						url2:"../../../static/img/weizhi2.png",
						name1:"商品名称",
						name2:"搜索抓到的sku名称",
						name3:"母猪产品鲜品",
						name4:"中国-厂家名称",
						name5:"张三信息科技有限公司",
						name6:"￥35/千克",
						name7:"100km",
						name8:"进店",
					},
					{
						url1:"../../../static/img/roo2.png",
						url2:"../../../static/img/weizhi2.png",
						name1:"商品名称",
						name2:"搜索抓到的sku名称",
						name3:"母猪产品鲜品",
						name4:"中国-厂家名称",
						name5:"张三信息科技有限公司",
						name6:"￥15/千克",
						name7:"100km",
						name8:"进店",
					},
					{
						url1:"../../../static/img/roo2.png",
						url2:"../../../static/img/weizhi2.png",
						name1:"商品名称",
						name2:"搜索抓到的sku名称",
						name3:"母猪产品鲜品",
						name4:"中国-厂家名称",
						name5:"张三信息科技有限公司",
						name6:"￥15/千克",
						name7:"100km",
						name8:"进店",
					},
				],
				active:1,
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
</style>