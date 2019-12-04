<template>
	<view class="bgColor he">
		<view class="bankcard">
			<view class="list zs">
				<view class="account">
					<image src="../../../static/image/gsyh.png" mode=""></image>
					<view class="yh">
						<text class="title">中国建设银行<text>储蓄卡</text></text>
						<text class="kh">＊＊＊＊<text>0871</text></text>
					</view>
				</view>
				<text class="remove">解除绑定</text>
			</view>
			<view class="list gs">
				<view class="account">
					<image src="../../../static/image/zsyyhk.png" mode=""></image>
					<view class="yh">
						<text class="title">中国工商银行<text>储蓄卡</text></text>
						<text class="kh">＊＊＊＊<text>0856</text></text>
					</view>
				</view>
				<text class="remove">解除绑定</text>
			</view>
			<view class="list gs">
				<view class="account">
					<image src="../../../static/image/zsyyhk.png" mode=""></image>
					<view class="yh">
						<text class="title">招商银行<text>储蓄卡</text></text>
						<text class="kh">＊＊＊＊<text>0912</text></text>
					</view>
				</view>
				<text class="remove">解除绑定</text>
			</view>
		</view>
		<view class="textNext">
			<!-- 只能用到微信小程序中 -->
			<!--#ifdef MP-WEIXIN-->
			<button type="button" class="loguin">添加银行卡</button>
			 <!-- #endif -->
			 <!--除微信小程序平台其它平台都可以用 -->
			 <!--#ifndef MP-WEIXIN-->
			 <button type="primary">添加银行卡</button>
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
	margin: 0 auto;
	margin-top: 100upx;
}
.bankcard{
	margin-top: 60upx;
}
.bankcard .list{
	height: 218upx;
	display: flex;
	justify-content: space-between;
	align-items: center;
	margin: 0 30upx;
	border-radius: 20upx;
	padding: 0 30upx;
	margin-bottom: 20upx;
}
.bankcard .list .account{
	display: flex;
}
.bankcard .list .yh{
	display: flex;
	flex-direction: column;
}
.bankcard .list image{
	width: 100upx;
	height:100upx;
	margin-right: 30upx;
}
.bankcard .list  .account .yh{
	color: #fff;
}
.bankcard .list  .account .title{
	font-size: 40upx;
}
.bankcard .list  .account .title text{
	font-size: 26upx;
	margin-left: 30upx;
}
.bankcard .list  .account .kh{
	margin-top: 10upx;
	font-size: 24upx;
}
.bankcard .list  .account .kh text{
	font-size: 36upx;
	margin-left: 30upx;
}
.bankcard .list .remove{
	color: #FFFFFF;
	font-size: 28upx;
	margin-top: 80upx;
}
.gs{
	background:linear-gradient(to right,#ff7566,#ff6364,#fe5262)
}
.zs{
	background:linear-gradient(to right,#54a9ee,#437ed1,#3a63be)
}
</style>
