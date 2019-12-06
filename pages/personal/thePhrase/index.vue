<template>
	<view class="bgColor he">
		<view class="phrase">
			<view class="list">
				<text>请问你不舒服多久了？</text>
			</view>
			<view class="list">
				<text>请问你最近症状有所改善么？具体哪些方面？</text>
			</view>
			<view class="list">
				<text>请问最近是在孕期么？</text>
			</view>
			<view class="list">
				<text>悲剧啊华盛顿附近开v会附近开吧你的疯狂了睡觉啊吧是好噶数据有点过分和v句都是伴侣阿道夫v和精雕细琢。</text>
			</view>
			<view class="list">
				<text>悲剧啊华盛顿附近开v会真的v吧你的疯狂了睡觉啊吧是噶数据有点过分和附近开悲剧啊华盛顿附近开v悲剧啊华悲剧啊华盛顿附近开v悲剧啊华盛顿盛顿附近开。</text>
			</view>
		</view>
		<view class="textNext">
			<!-- 只能用到微信小程序中 -->
			<!--#ifdef MP-WEIXIN-->
			<button type="button" class="loguin" @tap="add">添加常用语</button>
			 <!-- #endif -->
			 <!--除微信小程序平台其它平台都可以用 -->
			 <!--#ifndef MP-WEIXIN-->
			 <button type="primary" @tap="add">添加常用语</button>
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
			add() {
				uni.navigateTo({
					url: '/pages/personal/thePhrase/add'
				});
			}	
		}
	}
</script>

<style>
.phrase{
	background: #FFFFFF;
	margin-top: 30upx;
}
.phrase .list{
	display: flex;
	padding:30upx;
	border-bottom:1upx solid #e4e4e4;
	font-size: 28upx;
	color: #4a4a4a;
}
.phrase .list:last-child{
	border-bottom:none;
}
.textNext{
	width: 90%;
	margin: 0 auto;
	padding-top: 300upx;
}
</style>
