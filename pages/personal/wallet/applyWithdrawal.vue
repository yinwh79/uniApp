<template>
	<view class="bgColor he">
		<view class="choose">
			<view class="information-text-title">
				<image src="../../../static/image/zsyyhk.png" mode="" class="yh"></image>
				<view class="information-text">
					<view class="title">
						招商银行
						<text>储蓄卡</text>
					</view>
					<view class="cardNumber">
						**** **** **** 
						<text>5309</text>
					</view>
				</view>
			</view>
			<image src="../../../static/image/arrow.png" mode="" class="arrows"></image>
		</view>
		<view class="Withdrawalamount">
			<view class="Withdrawalamount-center">
				<view class="logins">
					<image src="../../../static/image/mount.png" mode=""></image>
					<text>提现金额</text>
				</view>
				<view class="inputtext">
					<image src="../../../static/image/inputmoun.png" mode=""></image>
					<input type="text" value="" />
				</view>
			</view>
			<view class="limit">
				<text>账户余额: ￥500.00  可提现金额: 400.00</text>
			</view>
		</view>
		<view class="textNext">
			<!-- 只能用到微信小程序中 -->
			<!--#ifdef MP-WEIXIN-->
			<button type="button" class="loguin">确认提现</button>
			 <!-- #endif -->
			 <!--除微信小程序平台其它平台都可以用 -->
			 <!--#ifndef MP-WEIXIN-->
			 <button type="primary">确认提现</button>
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
.textNext{
	width: 90%;
	margin: 100upx auto 0;
}
.choose{
	margin-top: 30upx;
	display: flex;
	align-items: center;
	justify-content: space-between;
	padding: 0 30upx;
	background: #FFFFFF;
	border-bottom: 1upx solid #e6e6e6;
}
.choose .yh{
	width: 100upx;
	height: 100upx;
	margin-right: 30upx;
}
.choose .information-text-title{
	display: flex;
	flex-direction: row;
	align-items: center;
	height: 147upx;
}
.choose .title{
	font-size: 32upx;
	color: #333333;
}
.choose .title text{
	font-size: 28upx;
	color: #999999;
	margin-left: 30upx;
}
.choose .cardNumber{
	font-size: 32upx;
	color: #333333;
	margin-top: 10upx;
}
.Withdrawalamount{
	margin: 25upx 30upx;
}
.Withdrawalamount .Withdrawalamount-center{
	background-color: #FFFFFF;
	border-radius: 20upx;
	padding-bottom: 30upx;
}
.Withdrawalamount .Withdrawalamount-center .logins{
	display: flex;
	padding:25upx 0 0 30upx;
	align-items: center;
}
.Withdrawalamount .Withdrawalamount-center .logins image{
	width: 54upx;
	height: 54upx;
	margin-right: 20upx;
}
.Withdrawalamount .Withdrawalamount-center .logins text{
	font-size: 32upx;
	color: #333333;
	margin-right: 17upx;
}
.Withdrawalamount .Withdrawalamount-center .inputtext{
	margin-top: 32upx;
	margin-left: 90upx;
	display: flex;
	align-items: center;
}
.Withdrawalamount .Withdrawalamount-center .inputtext image{
	width: 68upx;
	height: 84upx;
	margin-right: 20upx;
	flex-shrink: 0;
}
.Withdrawalamount .Withdrawalamount-center .inputtext input{
	height: 126upx;
	font-size: 100upx;
}
.Withdrawalamount .limit{
	font-size: 26upx;
	color: #999999;
	margin-top: 27upx;
}
</style>
