<template>
	<view class="bgColor he">
		<view class="addzyd">
			<view class="list">
				<text>多点执业医院</text>
				<input type="text" value="" placeholder="请输入医院" placeholder-style="color:#cccccc;"/>
			</view>
			<view class="list">
				<text>科室</text>
				<input type="text" value="" placeholder="请输入科室" placeholder-style="color:#cccccc;"/>
			</view>
			<view class="list">
				<text>省 / 市 / 区</text>
				<input type="text" value="" placeholder="省-市-区" placeholder-style="color:#cccccc;"/>
			</view>
			<view class="list">
				<text>医院地址</text>
				<input type="text" value="" placeholder="请输入医院详细地址" placeholder-style="color:#cccccc;"/>
			</view>
		</view>
		<view class="textNext">
			<!-- 只能用到微信小程序中 -->
			<!--#ifdef MP-WEIXIN-->
			<button type="button" class="loguin" @tap="nextPag">确定</button>
			 <!-- #endif -->
			 <!--除微信小程序平台其它平台都可以用 -->
			 <!--#ifndef MP-WEIXIN-->
			 <button type="primary" @tap="nextPag">确定</button>
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
.addzyd{
	margin-top: 30upx;
}
.addzyd .list{
	display: flex;
	align-items: center;
	font-size: 28upx;
	border-bottom: 1upx solid #e4e4e4;
	height: 100upx;
	background-color: #FFFFFF;
	padding: 0 30upx;
}
.addzyd .list:last-child{
	border-bottom:none;
}
.addzyd .list text{
	width: 190upx;
	display: inline-block;
	color: #4a4a4a;
}
.textNext{
	padding-top: 300upx;
	width: 90%;
	margin: 0 auto;
}
</style>
