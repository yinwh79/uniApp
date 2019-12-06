<template>
	<view class="bgColor he">
		<view class="professional">
			<view class="list">
				<view class="listrightTit">
					<image src="../../../static/image/point01.png" mode=""></image>
					<view class="rightTit">
						<view class="title">
							<text class="name">重庆铭博医院</text>
							<text>内科</text>
						</view>
						<text class="foot-title">重庆冉家坝***路**号</text>
					</view>
				</view>
			</view>
			<view class="list">
				<view class="listrightTit">
					<image src="../../../static/image/point02.png" mode=""></image>
					<view class="rightTit">
						<view class="title">
							<text class="name">重庆铭博医院</text>
							<text>内科</text>
						</view>
						<text class="foot-title">重庆冉家坝***路**号</text>
					</view>
				</view>
				<view class="delet">
					<text>删除</text>
				</view>
			</view>
			<view class="list">
				<view class="listrightTit">
					<image src="../../../static/image/point02.png" mode=""></image>
					<view class="rightTit">
						<view class="title">
							<text class="name">重庆铭博医院</text>
							<text>内科</text>
						</view>
						<text class="foot-title">重庆冉家坝***路**号</text>
					</view>
				</view>
				<view class="delet">
					<text>删除</text>
				</view>
			</view>
		</view>
		<view class="textNext">
			<!-- 只能用到微信小程序中 -->
			<!--#ifdef MP-WEIXIN-->
			<button type="button" class="loguin" @tap="nextPag">添加执业点</button>
			 <!-- #endif -->
			 <!--除微信小程序平台其它平台都可以用 -->
			 <!--#ifndef MP-WEIXIN-->
			 <button type="primary" @tap="nextPag">添加执业点</button>
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
				uni.navigateTo({
				    url: '/pages/personal/professional/add'
				});
			}
		}
	}
</script>

<style>
.professional{
	margin: 47upx 30upx 0;
}
.professional .list{
	box-shadow:0px 0px 6px #eaeaea;
	display: flex;
	background-color: #FFFFFF;
	border-radius: 20upx;
	align-items: center;
	justify-content: space-between;
	height: 180upx;
	margin-top: 20upx;
	padding: 0 30upx;
}
.professional .listrightTit{
	display: flex;
	flex-direction: row;
	align-items: center;
}
.professional .delet{
	color: #fc2702;
	font-size: 26upx;
	margin-top: 60upx;
}
.professional .list image{
	width: 119upx;
	height: 119upx;
	margin-right: 20upx;
}
.professional .list .rightTit{
	display: flex;
	flex-direction: column;
}
.professional .list .rightTit .title .name{
	font-size: 40upx;
	color: #000000;
	margin-right: 30upx;
	
}
.professional .list .rightTit .title text{
	font-size: 26upx;
}
.professional .list .foot-title{
	font-size: 30upx;
	color: #999999;
}
.textNext{
	width: 90%;
	margin: 0 auto;
	padding-top: 200upx;
	
}
</style>
