<template>
	<view class="bgColor he">
		<view class="headerMoney">
			<text class="text">总收入积分</text>
			<text class="money">360</text>
			<view class="date">
				<image src="../../../static/image/dataTime.png" mode="" class="dataTim"></image>
				<text>2019 . 08</text>
			</view>
		</view>
		<view class="list-money list-price">
			<view class="list">
				<view class="textarr">
					<text>图文咨询</text>
					<text class="date">2019-02-11</text>
				</view>
				<view class="price">
					<text>30.00</text>
					<image src="../../../static/image/arrow.png" mode="" class="gd"></image>
				</view>
			</view>
			<view class="list">
				<view class="textarr">
					<text>图文咨询</text>
					<text class="date">2019-02-08</text>
				</view>
				<view class="price">
					<text>30.00</text>
					<image src="../../../static/image/arrow.png" mode="" class="gd"></image>
				</view>
			</view>
			<view class="list">
				<view class="textarr">
					<text>视频咨询</text>
					<text class="date">2019-02-11</text>
				</view>
				<view class="price">
					<text>30.00</text>
					<image src="../../../static/image/arrow.png" mode="" class="gd"></image>
				</view>
			</view>
		</view>
		<view class="textNext">
			<!-- 只能用到微信小程序中 -->
			<!--#ifdef MP-WEIXIN-->
			<button type="button" class="loguin">申请提现</button>
			 <!-- #endif -->
			 <!--除微信小程序平台其它平台都可以用 -->
			 <!--#ifndef MP-WEIXIN-->
			 <button type="primary">申请提现</button>
			 <!-- #endif -->
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
.headerMoney{
	display: flex;
	flex-direction: column;
	align-items: center;
	background-color: #FFFFFF;
	padding: 35upx 0;
	margin-top: 30upx;
}
.headerMoney .text{
	font-size: 30upx;
	color: #999999;
}
.headerMoney .money{
	font-size: 80upx;
	color: #f98e47;
}
.headerMoney .date .dataTim{
	width: 33upx;
	height: 32upx;
	margin-right: 20upx;
}
.headerMoney .date{
	color: #333333;
	font-size: 36upx;
}
.list-price .textarr text:last-child{
	font-size: 24upx;
	color: #cccccc;
}
.list-price .textarr text:first-child{
	font-size: 28upx;
	color: #4a4a4a;
	margin-right: 30upx;
}
.list-price .price text{
	font-size: 28upx;
	color: #4a4a4a;
	margin-right: 20upx;
}
.textNext{
	width: 90%;
	margin: 100upx auto 0;
}
</style>
