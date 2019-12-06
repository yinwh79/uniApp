<template>
	<view class="bgColor he">
		<view class="heads-income">
			<view class="text">
				收益
				<text> + 360</text>
			</view>
		</view>
		<view class="action-text">
			<view class="list">
				<view class="lf">交易类型</view>
				<view class="rf">图文咨询</view>
			</view>
			<view class="list">
				<view class="lf">详情</view>
				<view class="rf">王立体购买了图文咨询</view>
			</view>
			<view class="list">
				<view class="lf">订单总额</view>
				<view class="rf">￥30.00</view>
			</view>
			<view class="list">
				<view class="lf">退款金额</view>
				<view class="rf">￥10.00</view>
			</view>
			<view class="list">
				<view class="lf">退款时间</view>
				<view class="rf">2019-10-02  05:48</view>
			</view>
			<view class="list">
				<view class="lf">订单号</view>
				<view class="rf">a2019071818100</view>
			</view>
			<view class="list">
				<view class="lf">支付流水号</view>
				<view class="rf">DD2019071818100001</view>
			</view>
			<view class="list">
				<view class="lf">支付时间</view>
				<view class="rf">2019-10-02  02:48</view>
			</view>
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
.heads-income{
	background-color: #FFFFFF;
	display: flex;
	justify-content: center;
	align-items: center;
	height: 173upx;
	margin-top: 30upx;
	font-size: 43upx;
	color: #333333;
}
.heads-income .text{
	display: flex;
	align-items: center;
}
.heads-income .text text{
	font-size: 80upx;
	color: #f98e47;
	padding-left: 20upx;
}
.action-text{
	background-color: #FFFFFF;
	margin-top: 30upx;
}
.action-text .list{
	height: 87upx;
	display: flex;
	align-items: center;
	justify-content: space-between;
	border-bottom: 1upx solid #e4e4e4;
}
.action-text .list:last-child{
	border-bottom: none;
}
.action-text .list .lf{
	width: 199upx;
	border-right: 1upx solid #e4e4e4;
	height: 87upx;
	font-size: 28upx;
	color: #4a4a4a;
	margin-left: 28upx;
	line-height: 87upx;
}
.action-text .list .rf{
	margin-right: 28upx;
	color: #4a4a4a;
	font-size: 28upx;
}
</style>
