<template>
	<view class="bgColor he">
		<view class="integral">
			<view class="money">
				<text class="text">账户剩余积分</text>
				<text class="balance">360</text>
			</view>
			<view class="detail">
				<view class="">
					<text class="title">200</text>
					<text class="text">总收入积分</text>
				</view>
				<view class="dbsob">
					<text class="title">500</text>
					<text class="text">已提现积分</text>
				</view>
				<view class="">
					<text class="title">200</text>
					<text class="text">冻结中积分</text>
				</view>
			</view>
		</view>
		<view class="list-money">
			<view class="list" @tap="incomeDetails">
				<text>收入明细</text>
				<image src="../../../static/image/arrow.png" mode="" class="gd"></image>
			</view>
			<view class="list" @tap="Withdrawal">
				<text>提现记录</text>
				<image src="../../../static/image/arrow.png" mode="" class="gd"></image>
			</view>
			<view class="list" @tap="bankCard">
				<text>我的银行卡</text>
				<image src="../../../static/image/arrow.png" mode="" class="gd"></image>
			</view>
		</view>
		<view class="textNext">
			<!-- 只能用到微信小程序中 -->
			<!--#ifdef MP-WEIXIN-->
			<button type="button" class="loguin" @tap="nextPag">申请提现</button>
			 <!-- #endif -->
			 <!--除微信小程序平台其它平台都可以用 -->
			 <!--#ifndef MP-WEIXIN-->
			 <button type="primary" @tap="nextPag">申请提现</button>
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
			incomeDetails() {
				uni.navigateTo({
				    url: '/pages/personal/wallet/theDetail'
				});
			},
			Withdrawal() {
				uni.navigateTo({
				    url: '/pages/personal/wallet/withdrawal'
				});
			},
			bankCard() {
				uni.navigateTo({
				    url: '/pages/personal/wallet/bankCard'
				});
			}
		}
	}
</script>

<style>
.integral {
	margin-top: 30upx;
	background-color: #FFFFFF;
	padding-top: 30upx;
}
.integral .money{
	display: flex;
	flex-direction: column;
	align-items: center;
}
.integral .money .text{
	font-size: 30upx;
	color: #999999;
}
.integral .money .balance{
	font-size:80upx;
	color:#f98e47;
}
.detail{
	display: flex;
	justify-content: space-around;
	padding: 30upx 0;
}
.detail .dbsob{
	border-left: 1upx solid #dddddd;
	border-right: 1upx solid #dddddd;
}
.detail view{
	display: flex;
	flex-direction: column;
	align-items: center;
	width: 100%;
}
.detail .title{
	font-size: 44upx;
	color: #f98e47;
}
.detail .text{
	font-size: 30upx;
	color: #999999;
	margin-top: 10upx;
}
.textNext{
	width: 90%;
	margin: 100upx auto 0;
}
</style>
