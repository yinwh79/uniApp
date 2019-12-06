<template>
	<view class="bgColor he">
		<view class="textareaadd">
			<textarea value="悲剧啊华盛顿附近开会真的v吧你的疯狂了睡觉啊吧数据有点过分和附近开悲剧啊华盛顿附近开悲剧啊悲剧啊华盛顿附近开v悲剧据有点过分和附近开悲剧啊华盛顿附近开悲剧啊悲剧啊华盛顿附近开v悲剧啊华盛顿盛顿附近开。" placeholder="请输入" />
		</view>
		<view class="textNext">
			<!-- 只能用到微信小程序中 -->
			<!--#ifdef MP-WEIXIN-->
			<button type="button" class="loguin" @tap="nextPag">添加</button>
			 <!-- #endif -->
			 <!--除微信小程序平台其它平台都可以用 -->
			 <!--#ifndef MP-WEIXIN-->
			 <button type="primary" @tap="nextPag">添加</button>
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
			nextPag() {
				uni.navigateBack({
				    delta: 1
				});
			}
		}
	}
</script>

<style>
.textareaadd{
	margin: 30upx;
	background: #FFFFFF;
	padding: 30upx;
}
.textareaadd textarea{
	width: 100%;
	color: #4a4a4a;
	font-size: 28upx;
	line-height: 40upx;
}
.textNext{
	width: 90%;
	margin: 0 auto;
	padding-top: 300upx;
}
</style>
