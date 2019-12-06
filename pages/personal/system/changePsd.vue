<template>
	<view class="he">
		<view class="changepsd">
			<text>账号</text>
			<text>15879586587</text>
		</view>
		<view class="passwod">
			<view class="lists">
				<text>原 密 码</text>
				<input type="text" value="" placeholder="请输入原密码" placeholder-style="color;#e4e4e4;"/>
			</view>
			<view class="lists">
				<text>新 密 码</text>
				<input type="text" value="" placeholder="请输入新密码" placeholder-style="color;#e4e4e4;"/>
			</view>
			<view class="lists">
				<text>确认密码</text>
				<input type="text" value="" placeholder="请再次输入新密码" placeholder-style="color;#e4e4e4;"/>
			</view>
			<view class="describe">
				<text>密码必须由8-16位数字、字符组合 (不能是纯数字）</text>
				<view class="">
					忘记密码？
				</view>
			</view>
		</view>
		<view class="textNext">
			<!-- 只能用到微信小程序中 -->
			<!--#ifdef MP-WEIXIN-->
			<button type="button" class="loguin">确认修改</button>
			 <!-- #endif -->
			 <!--除微信小程序平台其它平台都可以用 -->
			 <!--#ifndef MP-WEIXIN-->
			 <button type="primary">确认修改</button>
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
	margin: 300upx auto 0;
}
.changepsd{
	font-size: 30upx;
	color: #4a4a4a;
	height: 100upx;
	border-bottom: 30upx solid #f5f5f5;
	border-top: 30upx solid #f5f5f5;
	display: flex;
	justify-content: space-between;
	padding: 0 30upx;
	align-items: center;
}
.passwod .lists{
	display: flex;
	align-items: center;
	height: 100upx;
	border-bottom: 1upx solid #e5e5e5;
	margin: 0 30upx;
}
.passwod .lists text{
	font-size: 30upx;
	color: #1f1f1f;
	margin-right: 30upx;
	width: 120upx;
	display: inline-block;
}
.passwod .lists input{
	font-size: 30upx;
}
.describe{
	font-size: 30upx;
	margin-top: 23upx;
	padding: 0 30upx;
}
.describe text{
	color: #999999;
}
.describe view{
	margin-top: 10upx;
	color: #4d9dff;
}
</style>
