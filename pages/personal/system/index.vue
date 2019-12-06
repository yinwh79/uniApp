<template>
	<view class="bgColor he">
		<view class="systemStt">
			<view class="list">
				<text>账号</text>
				<text>18512389587</text>
			</view>
			<view class="list" @tap="ChangePsd">
				<text>修改密码</text>
				<image src="../../../static/image/arrow.png" mode="" class="arrows"></image>
			</view>
			<view class="list">
				<text>免打扰模式</text>
				<view class="">
					<switch style="transform:scale(0.7)"/>
				</view>
			</view>
			<view class="list">
				<text>关于我们</text>
				<text></text>
			</view>
		</view>
		<view class="textNext replace">
			<!-- 只能用到微信小程序中 -->
			<!--#ifdef MP-WEIXIN-->
			<button type="button" class="loguin" @tap="modify">更换手机号</button>
			 <!-- #endif -->
			 <!--除微信小程序平台其它平台都可以用 -->
			 <!--#ifndef MP-WEIXIN-->
			 <button type="primary" @tap="modify">更换手机号</button>
			 <!-- #endif -->
		</view>
		<view class="textNext">
			<!-- 只能用到微信小程序中 -->
			<!--#ifdef MP-WEIXIN-->
			<button type="button" class="loguin">退出登录</button>
			 <!-- #endif -->
			 <!--除微信小程序平台其它平台都可以用 -->
			 <!--#ifndef MP-WEIXIN-->
			 <button type="primary">退出登录</button>
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
			modify() {
				uni.navigateTo({
				    url: '/pages/personal/system/modify/index'
				});
			},
			ChangePsd() {
				uni.navigateTo({
				    url: '/pages/personal/system/changePsd'
				});
			}
		}
	}
</script>

<style>
.systemStt{
	margin-top: 30upx;
	background-color: #FFFFFF;
}
.systemStt .list{
	margin: 0 30upx;
	display: flex;
	align-items: center;
	justify-content: space-between;
	height: 100upx;
	border-bottom: 1upx solid #e4e4e4;
	padding: 0 10upx;
	font-size: 28upx;
	color: #4a4a4a;
}
.replace{
	padding-top: 200upx;
	padding-bottom: 80upx;
}
.replace button{
	background-color: #767afd;
}
.textNext{
	width: 90%;
	margin: 0 auto;
}
</style>
