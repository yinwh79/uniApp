<template>
	<view class="bgColor">
		<view class="addgroup">
			<text class="name">名称</text>
			<input type="text" value="糖尿病" />
		</view>
		<view class="textNext">
			<!-- 只能用到微信小程序中 -->
			<!--#ifdef MP-WEIXIN-->
			<button type="button" class="loguin" @tap="nextPag">完成</button>
			 <!-- #endif -->
			 <!--除微信小程序平台其它平台都可以用 -->
			 <!--#ifndef MP-WEIXIN-->
			 <button type="primary" @tap="nextPag">完成</button>
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
	.bgColor{
		height: 100vh;
		overflow: hidden;
	}
.addgroup{
	background-color: #FFFFFF;
	height: 100upx;
	padding: 0 30upx;
	display: flex;
	align-items: center;
	margin-top: 30upx;
}
.addgroup .name{
	color:#999999 ;
	font-size: 32upx;
	margin-right: 30upx;
}
.textNext{
	margin: 0 auto;
	left: 0;
	right: 0;
	position: absolute;
	bottom: 100upx;
	width: 90%;
}
</style>
