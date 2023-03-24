<template>
	<view class="address">
		<view class="address-box"></view>
		<view class="address-bom">
			<view class="address-bom-text">
				联系人：
			</view>
			<input class="address-bom-input" type="text" placeholder="张晓伟">
		</view>
		<view class="address-bom1">
			<view class="address-bom-text">
				手机号：
			</view>
			<input class="address-bom-input" type="text" placeholder="18627821923">
		</view>
		<view class="address-bom1">
			<view class="address-bom-text">
				地区：
			</view>
			<input class="address-bom-input" type="text" placeholder="请选择" @click="tanchu">
			<u-picker :show="show" ref="uPicker" :columns="columns" @confirm="confirm" @change="changeHandler"></u-picker>
		</view>
		<view class="address-bom2">
			<view class="address-bom-text">
				详细地址：
			</view>
			<input class="address-bom-input" type="text" placeholder="请输入街道门牌号">
		</view>
		<view class="address-xz">
			<view>
				<image @click="iSshowStatus" v-if="iSshow == false" class="address-xz-img1" src="../../static/img/yuan1.png" alt="">
			</view>
			<view>
				<image @click="iSshowStatus" v-if="iSshow == true" class="address-xz-img2" src="../../static/img/yuan2.png" alt="">
			</view>
			<view class="address-xz-text">
				默认选中
			</view>
		</view>
		<view class="address-xz-btn">
			保存
		</view>
	</view>
</template>

<script>
	export default{
		data(){
			return{
				iSshow:false,
				show: false,
				columns: [
				            ['中国', '美国'],
				            ['深圳', '厦门', '上海', '拉萨']
						],
				columnData: [
				            ['深圳', '厦门', '上海', '拉萨'],
				            ['得州', '华盛顿', '纽约', '阿拉斯加']
				        ]
							
			}
		},
		methods:{
			iSshowStatus(){
				this.iSshow =! this.iSshow
			},
			tanchu(){
				this.show =! this.show
			},
			changeHandler(e) {
			                const {
			                    columnIndex,
			                    value,
			                    values, // values为当前变化列的数组内容
			                    index,
								// 微信小程序无法将picker实例传出来，只能通过ref操作
			                    picker = this.$refs.uPicker
			                } = e
			                // 当第一列值发生变化时，变化第二列(后一列)对应的选项
			                if (columnIndex === 0) {
			                    // picker为选择器this实例，变化第二列对应的选项
			                    picker.setColumnValues(1, this.columnData[index])
			                }
			            },
						// 回调参数为包含columnIndex、value、values
						confirm(e) {
			                console.log('confirm', e)
			                this.show = false
						}
		}
	}
	
</script>

<style>
	.address-box{
		width: 100%;
		height: 20rpx;
	}
	.address{
		height: 1624rpx;
		background: #F5F5F5;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
	}
	.address-bom{
		height: 84rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		display: flex;
		align-items: center;
		border-bottom: 2rpx solid #f8f8f8;
	}
	.address-bom1{
		height: 84rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		display: flex;
		align-items: center;
		border-bottom: 2rpx solid #f8f8f8;
	}
	.address-bom2{
		height: 84rpx;
		background: #FFFFFF;
		border-radius: 0rpx 0rpx 0rpx 0rpx;
		opacity: 1;
		display: flex;
		align-items: center;
	}
	.address-bom-text{
		/* width: 128rpx; */
		height: 44rpx;
		font-size: 32rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #333333;
		line-height: 38rpx;
		margin-left: 50rpx;
	}
	.address-bom-input{
		/* width: 84rpx; */
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Medium, PingFang SC;
		font-weight: 500;
		color: #999999;
		line-height: 33rpx;
	}
	.address-xz{
		display: flex;
		align-items: center;
		margin-top: 34rpx;
		margin-left: 22rpx;
	}
	.address-xz-img1{
		width: 48rpx;
		height: 48rpx;
	}
	.address-xz-img2{
		width: 48rpx;
		height: 48rpx;
	}
	.address-xz-text{
		width: 112rpx;
		height: 40rpx;
		font-size: 28rpx;
		font-family: PingFang SC-Regular, PingFang SC;
		font-weight: 400;
		color: #999999;
		line-height: 33rpx;
		margin-left: 8rpx;
	}
	.address-xz-btn{
		width: 690rpx;
		height: 88rpx;
		line-height: 88rpx;
		text-align: center;
		background: #3891ED;
		border-radius: 200rpx 200rpx 200rpx 200rpx;
		opacity: 1;
		margin-top: 104rpx;
		margin-left: 30rpx;
		font-family: PingFang SC-Medium;
		font-weight: Medium;
		font-size: 32rpx;
		color: #FFFFFF;
	}
</style>