<template>
	<view class="bgColor he">
		<view class="headewithdrawal">
			 <text class="thentext">已转帐</text>
			 <text class="theprice">50360.00</text>
		</view>
		<view class="withdrawaldetails">
			<view class="lists">
				<text>申请时间</text>
				<text>2019-10-02  05:48</text>
			</view>
			<view class="lists">
				<text>审核时间</text>
				<text></text>
			</view>
			<view class="lists">
				<text>转账时间</text>
				<text></text>
			</view>
		</view>
		<view class="titlewithdeawal">
			<text>以银行卡实际到账时间为准!</text>
		</view>
		<view class="describeRem">
			<text>审核描述</text>
			<text class="">转成成功</text>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			
		}
	}
</script>

<style>
.headewithdrawal{
	background-color: #FFFFFF;
	margin-top: 30upx;
	display: flex;
	align-items: center;
	height: 197upx;
	flex-direction: column;
	padding-top: 35upx;
}
.headewithdrawal .thentext{
	font-size: 30upx;
	color: #999999;
}
.headewithdrawal .theprice{
	font-size: 80upx;
	color: #f98e47;
}
.withdrawaldetails{
	background-color: #FFFFFF;
	font-size: 28upx;
	color: #4a4a4a;
	margin-top: 30upx;
}
.withdrawaldetails .lists{
	height: 100upx;
	display: flex;
	align-items: center;
	justify-content: space-between;
	border-bottom: 1upx solid #e4e4e4;
	margin: 0 23upx;
	padding: 0 15upx;
}
.withdrawaldetails .lists:last-child{
	border-bottom: none;
}
.titlewithdeawal{
	font-size: 24upx;
	color: #999999;
	padding: 20upx 0 20upx 30upx;
}
.describeRem{
	font-size: 28upx;
	color: #4a4a4a;
	height: 100upx;
	display: flex;
	justify-content: space-between;
	align-items: center;
	background-color: #FFFFFF;
	padding: 0 30upx;
}
.describeRem .miaos{
	color: #fc2702;
}
</style>
